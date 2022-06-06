## Week 10 lab report 5
Q1
I firstly  run the bash file and save the result of the lab9 code and result of my code as different txt files. 
Then I use the vim diff to find the different lines in the file. 
After that, I go back to the result of bash for loop and find which test file it is.
 
Q2
https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md
https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md
 
Q3
  1. For the 194.md,both my code the lab9 code is also incorrect
    As we can see the image, md preview recognize `Foo*bar`, and the corrct oput should be `[title (with parens)]` 
    ![e5cb4e83ac61aea7941a6919887933b](https://user-images.githubusercontent.com/103226676/172101640-25321d54-2cb1-40a5-baf0-b8492ca51373.png)
     
    However, my code give an empty array
     
    ![5b1c536721e9f6dd51a2e7c73f6cf30](https://user-images.githubusercontent.com/103226676/172102161-e65468de-8da1-469e-9113-f77638e2bd3b.png)
     
    And lab 9 code give a worng array
     
    ![d4a03964682e55a57ad6f28e4eca995](https://user-images.githubusercontent.com/103226676/172102253-809e24b4-d368-4a51-9995-214e12f06856.png)
    
    I think the problem of the lab9 code is need to check whether there is any thing between closeBrackets and openParen. 
     
    ![855f5ed267996705054e42a051099f3](https://user-images.githubusercontent.com/103226676/172103932-f85a197f-d505-4217-b5dc-bb56126eaf00.png)
    
    I think my problem is need to check this type of the link. `[]:(fileName) 'link' []` . When I write my code, I only consider `[]()` as a link
    and don't know the filename link part. As we can see the hight light part, only consider the bracket and parenthesis
     
    ![87ade02af3a5be000324c3a5289eb8f](https://user-images.githubusercontent.com/103226676/172105291-71862fa6-7b69-4431-9d23-0c485dbd8baf.png)

  2. For the 201.md. my code is right and lab9 code is incorrect
    As we can see the image, md preview doesn't recognize link
     
    ![eb894236b7c336f96b0f2bb4c407825](https://user-images.githubusercontent.com/103226676/172105649-7c7d35b1-3872-4589-aa20-ac4be883d2f9.png)
     
    My code give the empty array which is correct
     
    ![5b1c536721e9f6dd51a2e7c73f6cf30](https://user-images.githubusercontent.com/103226676/172105845-888f3b03-b8e8-427f-a052-b0c3783abe0e.png)
     
    Lab 9 code recognize baz as the link which is incorrect
     
    ![d4a03964682e55a57ad6f28e4eca995](https://user-images.githubusercontent.com/103226676/172105964-01a4d537-c286-4134-8233-6c59666fa301.png)
    
    I think the problem of the lab code is not recognize the correct index of the close paren. Nothing shoud between the closeBracket and OpenParen
     
    ![855f5ed267996705054e42a051099f3](https://user-images.githubusercontent.com/103226676/172106616-e577d77f-2e8c-4eb5-913d-ef89cdf63060.png)



    
    
