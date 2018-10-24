---
layout: page
--- 

## October 24: Texts

### Introduction

This week we're going to learn how to work with digitized historical text. In Part I you will explore the process of digitizing text itself. In Part II you will learn how to process text and turn it into data. In Part III you apply some of the skills you learned in the Voyant tutorial to do some basic text analysis. To learn these skills, we will be looking at a common type of historical document: newspapers.

### Part I: Text Databases

To understand how text gets stored in databases, we'll be examining one of the largest free archives of U.S. newspapers: the Library of Congress's Chronicling America database. This database allows users to search for newspapers published across the United States over more than one hundred years. But how does this textual database work and what goes on under the hood?

Navigate to the Advanced Search tab at Chronicling America: <https://chroniclingamerica.loc.gov/>. Perform a search that returns newspapers that were printed on Halloween in the year 1900. 

- How many results are there?
- Where are *three states* that are represented in these results?

Change your Advanced Search to narrow it down further: newspapers that were printed on Halloween in the year 1900, in the state of Minnesota, and that contain the word `halloween`. Copy and paste the resulting URL address from your results page into a plain text editor - typically TextEdit for Mac or Notepad for Windows. This type of URL acts as a set of instructions to the database that tells it was what kind of results to show you based on certain "parameters" (such as the date or state of publication). 

Re-paste a second version of the URL in your text editor and then try to modify the text so that if you load the URL in a web browser it returns newspapers that meet the following criteria:
  
- Printed on Christmas Day, one hundred years ago
- In the state of Arizona
- Containing the word `christmas`

**Hint**: your original URL probably has some confusing symbols. If you're having trouble, here is a cleaned-up version of the original URL that is easier to read and then modify to fit the above parameters: `https://chroniclingamerica.loc.gov/search/pages/results/?state=Minnesota&dateFilterType=range&date1=10/31/1900&date2=10/31/1900&ortext=halloween`

Once you have successfully changed the URL and gotten search results that match the above criteria, choose one of the newspapers from these results (don't just choose the first one) and zoom in to one of the mentions of `christmas`. Skim through the story. Now click on the `Text` link at the top of the viewer (next to `PDF`). Use your browser's find/search to try and relocate the story you just skimmed. Can you still understand it? Are any words difficult to understand? 

What you are seeing are the results of `Optical Character Recognition (OCR)` that we talked about earlier in the semester, in which a computer tries to "translate" a photographic *image* of text into *actual* text that you can analyze. 

Pause. If the other people in your group are still working on Part I and running into issues, offer to help. Once you have all completed Part I, share what you've found.

- What were the results of your particular paper?
- What are some of the implications that this OCR process might have for digital text analysis like the kind you read about for today? 
- How does this relate to some of the readings and themes from earlier weeks?
	
Check in with Cameron once you have finished Part I. 

### Part II: Processing Text

In this section, we're going to try and process and assemble text so that you can perform analysis on it. First, create a new folder on your computer named `week-8`. 

On the same page that shows the OCR'd version of your newspaper page (ex. <https://chroniclingamerica.loc.gov/lccn/sn84020558/1918-12-25/ed-1/seq-9/ocr/>, scroll down to the bottom of the page and click on the `txt` link. This is a link to a file that is *only* the raw, OCR'd text (and does not include any metadata. If you click on that link it will bring you to a URL that has ".txt" at the end. This means that your browser is showing you a text file rather than a webpage file (ex. if it ended in ".html").

Back in your browser, save the OCR text file into the `week-8` folder you created. Now you need to rename the file so that it tells you information about where it came from (its metadata). Instead of making up a name, go back to your browser and look at the URL. It should contain unique information that identifies which page, issue, and newspaper the text came from. 

- `sn84020558`: the unique ID of that newspaper title (ex. "The New York Times") 
- `1918-12-25`: the date of the issue
- `ed-1`: the edition
- `seq-9`: the page number (in this case, page 9). 

Rename the text file you just saved so that it includes this information, each separated by an underscore character ("_"). For the above example, this would look like `sn84020558_1918-12-25_ed-1_seq-9.txt`

Return to the browser. Try to alter the URL (ex. `https://chroniclingamerica.loc.gov/lccn/sn84020558/1918-12-25/ed-1/seq-9/ocr.txt`) so that it displays a text file of the *previous* page in that same issue (in this case, page 8 instead of page 9)? Note: if you are already on page 1, try doing the *next* page. Save the new page in the same format as you did above. Everything should look the same except for the number that comes after `seq-`.

You should now have two text files in your folder. We're going to combine these into one text larger text file by hand. But what if we had 2,000 files instead of 2 files? In that case, we would want to have the computer do this for us rather than copying and pasting them together by hand. This is fairly straightforward. For future reference: [PC users](https://www.computerhope.com/issues/ch001376.htm#merge-text) and [Mac Users](https://www.computerhope.com/unix/ucat.htm). For now, simply copy and paste your two files together into a new text (".txt") file.

Pause. If the other people in your group are still working on Part II and running into issues, offer to help. Once everyone has finished, check in with Cameron.

### Part III: Analyzing Text

Upload your new text file into Voyant. In your groups, divide up different tools in Voyant (areas of the screen interface). Each person go to [Voyant Help](https://voyant-tools.org/docs/#!/guide/start) and figure out what that tool is showing. Look at your example of a newspaper and see what it tells you. What sorts of patterns do you notice?

Go around and have each person explain what that particular tool does and what it is showing you about your text. Once everyone has presented, discuss: 

- Which of these tools seems most useful for historical research?
- How might the different tools be applied?
- What are their limitations?


