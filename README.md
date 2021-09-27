# RRC-Texas-G1-W2-GAU-Scanner
I made a video explaining the basics of how this program work. If you just want to run it all you need to do is make sure that you are read the API numbers from which ever document you are using correctly (I added a bit of text in the code describing this) (I would suggest you make a separate Excel document and copy paste the API's there because it will make reading it much easier for you). Next, make sure you step through all the cells and then call the main() function, this will start the reading. It takes two parameters (beginning, end). If you want to read from 0-300 (first 300 APIs) call main(0,300). 

There are three things you should be aware of: 
    
    1. The row list keeps track of the next row where each value (liner, GAU, Casing, etc.) needs to be written. If you reset this back to [2,2,2,2,2,2] it will mess up the order        of where it needs to write the next entry on the Excel document. Eventually I'll make it automatic so you don't worry about it but currently if you reset it it messes up          the order.  
    
    2. Be careful when running ClearData(). This resets the whole document and any reading  you made will be lost forever. Don't type it out unless you intend to reset the 
       document.  
    
    3. Any changes made to the document won't appear on the document until you run "wb.save("WellboreData.xlsx")". Don't be confused if you read 200 APIs and the data doesn't  
       appear on the document, you just need to run this and it will save it.   Few other things: 1. If you only want to read GAU Letters comment out lines 89 &amp; 83. If you  
       only want to read G1 documents comment out lines 83 &amp; 86. If you only want to read W2 documents comment out lines 86 &amp; 89.  2. If there is some weird unresolved
       error when reading a certain API number and it fails even if you run it again, just skip it and keep going (Try it again by calling main() with the beginning being the 
       index of that API number, if it doesn't work, add one to the beginning and keep going). 
  
YouTube Links:
 
 Video #1: https://www.youtube.com/watch?v=JRbr0TgahWk
 
 Video #2: https://www.youtube.com/watch?v=iI-kfChLHHA
 
