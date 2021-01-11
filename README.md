# xml-mp3-pt.2
Project 2 for Frank &lt;3 addendum to xml-mp3

XML project for Frank Akaiwa Fall 2020, grade: 100%

2 parts: XML data file, external schema

Rubric: 

Part A - Additional Content 
For this project you will create an XML Schema describing the structure and content of the XML document that you created for Project 1 (part C).   Before you get started with your schema you need to add some more information to the xml file.  
First, you need to add comments, ratings and genre for each of the artists and albums are a part of your XML document.  
•	Create a Comment element for each album in your xml file.  
In this element describe what you like or dislike about the album.  A short description is fine.  (Note: This is an actual XML element, I am not looking for a comment tag like this:  <!--  don’t put your comments about albums here.  -->
•	Create a Rating element or attribute for each of your albums with a rating value from 1 to 10 (1 is your least favorite and 10 is your most favorite).  You may treat this like a rank ordering of all the albums if you prefer, but it is not necessary. (In other words, it’s fine if you have 2 albums you really like and want to rate as 10.)
•	Create a Genre element or attribute for each artist or group. This information can be found on the www.allmusic.com website for each of your artists or groups.
Part B - XML Schema 
Based on the information contained in the XML document, create an XML Schema that restricts the content of following elements/attributes (in addition to describing the documents structure):
•	Artist or group: string values; required
•	Group members: string value, this can occur once, more than once or not at all
•	Genre: string value, must occur at least once per Artist or group; required 
•	Producers: string value, this can occur once, more than once or not at all
•	Engineers/Mixers: string value, this can occur once, more than once or not at all
•	Mastering Engineer: string value, this can occur once, more than once or not at all
•	Career Start or Career End: string value with a pattern matching the date formats in your xml file; optional 
•	Comment: string values, required length between 10 and 200 characters; optional
•	Album titles: string value, required
•	Album category: string values with choice of  “Grammy_Winner”, “Grammy_Nominee”, “Personal_Favorite”; required
•	Album rating: number with values between 1 and 10; required
•	Album release date: string value with a pattern matching the date formats in your xml file; optional
•	Country: string value; optional
•	Record label: string value; optional
•	Record label catalog no.: string value; optional
•	Bar Code No.: string value; optional
•	Format: string value with enumeration matching the values in your xml file; optional
•	Song position: integer, occurs only one time per track; required
•	Song title: string value, occurs only one time per track; required
•	Song length: string value with a pattern matching the time format MM:SS (Minutes may be displayed in single digits, but 2 digits must be allowed.  Seconds must be displayed with 2 digits), occurs only one time per track; required
•	Song Composers and writers: string value; optional
•	SKU: ID data type with a pattern matching K315F2020A for albums and K315F2020A001 for individual songs; required
•	Type: string values with a choice of album or song; required
o	Since this is used for both albums and songs, create a user-defined global definition in your schema named “productType”.
•	albumref: IDREF data type, with a pattern matching the album SKU; required for tracks
•	Album Picture File Name: string value with a pattern matching any file name with a file extension of .gif or .jpg or .jpeg or .png; required
•	Picture Source: string value, occurs only one time per album; required 
(Notes: If you have additional elements/attributes in your XML document feel free to define their structure/content however you feel is appropriate.  If you feel that you need to modify your XML document to complete this project feel free to do so; however, include a few sentences as a comment in your xml file explaining what you did and why you felt that it was necessary).

Save your XML document as username_project2.xml and your XML Schema as username_project2.xsd. 

Place the username_project2.xml and username_project2.xsd files in a compressed zip file named yourusername_project2.zip.  

Submit this file to the Individual Project 2 assignment on the Canvas site any time prior to the due date.
 
