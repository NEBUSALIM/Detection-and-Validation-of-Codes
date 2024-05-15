Exercise 1 : Detection and Validation of Codes
Problem Statement : 
•	Check images in folder IMG_20240508_*.jpg
•	Search codes included in ID_codes.txt file
•	Prepare two files:
o	Code existing in images, with image file name
o	Code not existing
Solution Abstract :
1.	Run a text detection and extraction algorithm on the images to get the code written in them.
2.	Compare the extracted codes with the codes given in the text file.
Tools/Packages Used:
•	Cv2
•	Numpy
•	Pytesseract
•	Matplotlib
Result :
1.	Successfully read the image.
2.	Converted the image to grayscale for text extraction
3.	Tried using Pytesseract to detect and extract the text from the images – but failed to fetch the text.
4.	The image was cropped to a single stack and the same was applied – but failed.
5.	The image was converted to binary for further analysis – it was found that the background colour of certain digits obscured detection in some columns.
 
Future Scope :
1.	Further analysis and optimisation is needed in the image pre-processing to effectively detect and extract the code from the images.
2.	A function is written to cross check the codes extracted from images with the codes in the text file. The corresponding lists are saved separately. The lists are written into separate files and saved. This can be tested only after the extraction of text.

