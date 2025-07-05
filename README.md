# Work with git and bash

## Task 1
File & Directory Operations (task covers basic terminal operations)

```javascript
% cd ~
% pwd
% mkdir test1
% cd test1
  test1 % touch file1.txt file2.txt file3.txt
  test1 % ls
  test1 % cd ~
% mkdir test2
% rmdir test2
% rm test1/file2.txt
% mkdir test3
% cp test1/file1.txt test3/
% cp test1/file3.txt test3/
% rm -r test3
% mkdir test4
% mv test1/file1.txt test4/
% mv test1/file3.txt test4/
% echo "line 1" >> test4/file1.txt
% echo "line 2" >> test4/file1.txt
% echo "line 3" >> test4/file1.txt
% cat test4/file1.txt
% echo "line 1" >> test4/file3.txt
% echo "line 2" >> test4/file3.txt
% echo "line 3" >> test4/file3.txt
%cat test4/file1.txt test4/file3.txt
% nano test4/file1.txt
%cat test4/file1.txt test4/file3.txt
```

## Task 2
Text Processing & Network Tools (task covers file management, pattern matching, and basic API testing using command-line tools)

```javascript
 % cd ~
 % mkdir test3 
 % echo -e "row1\nrow2\nrow3\nrow4" > test3/file4.txt
 % echo -e "row1\nrow2\nrow3\nrow4" > test3/file5.txt
 % echo -e "row1\nrow2\nrow3\nrow4" > test3/file6.txt
 % grep "row2" test3/file5.txt
 % grep "row" test3/*
 % grep -c "row" test3/file6.txt
 % find test3 -name "file5.txt"               
 % find test3 -name "file5.txt"
 % rm test3/file5.txt  
 % find test3 -name "file5.txt" -exec rm {} \;
 % echo "test" > test3/file4.txt
 % sed -i '' 's/test/fail/g' test3/file4.txt
 % echo "test" >> test3/file4.txt
 % ps -ef
 % kill 666
 % ping -c 4 rusau.net
 % curl -X GET "https://petstore.swagger.io/v2/pet/findByStatus?status=available"
 % curl -X POST "https://petstore.swagger.io/v2/user" \
  -H "accept: application/json" \
  -H "Content-Type: application/json" \
  -d '{"id":12345,"username":"newuser","firstName":"John","lastName":"Doe","email":"john@doe.com","password":"12345","phone":"1234567890","userStatus":1}'
{"code":200,"type":"unknown","message":"12345"}
```

## Task 3
Creating, cloning, pushing and pulling repositories

```javascript

git init lfedorishina                                       
git clone git@github.com:lfedorishina/lfedorishina.git      
git clone git@github.com:testrusau/testrusau.git            
cd testrusau                                                
git push git@github.com:lfedorishina/testrusau.git main:main
git commit -m "committed changes"                            
git push
```
