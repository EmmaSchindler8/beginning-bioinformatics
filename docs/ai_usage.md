# AI Use Log (Template) *really only needed for the Rosalind Problems*
- Tool/model & version:
- What I asked for:
- Snippet of prompt(s):
- What I changed before committing:
- How I verified correctness (tests, sample data):
# AI Use Log (1st Use)
- Tool/model & version: Gemini in Google Colab
- What I asked for: When trying to practice the code for Task 6.1 (Hello, "Enter name"...) I got an error. It asked me if it wanted AI Gemini to
  explain the code and I agreed.
- Snippet of prompt(s):Please explain this error: (the error was an STR)
- What I changed before committing:Nothing changed, AI said it fixed the error. Maybe I am missing something but the error is still there?
- How I verified correctness (tests, sample data): Spoke with TA Adam/Dr. Demuth.
# AI Use Log (2nd Use) 
- Tool/model & version: Gemini
- What I asked for: When working on problem 3, I was doing the example (sum the odd numbers from 100-200). I was getting a syntax erorr and and "expected :" error, so I accepted Gemini's help to explain the error. 
- Snippet of prompt(s):
  Me: Please explain this error: "SyntaxError: Expected ':'"
  Gemini: The error in the selected code is a SyntaxError: expected ':'. This means that the for loop is missing the colon at the end of the line. I will fix this by adding a colon at the end of the for loop line and then add the code to sum the odd numbers within the loop.
- What I changed before committing: I added in the word "for" for loop and changed the order of how I mentioned only wanting to sum odd numbers. I did not copy and paste or just accept the changes, I made note of them and re-wrote them myself to better learn/practice. Some did auto-populate as I typed. For example, I did not know originally I needed this line (sum_of_odds +=numbers), but Gemini explained to me it was needed because it adds the actual numbers to the sum
- How I verified correctness (tests, sample data): I used the test values from Rosalind (100, 200) and got the correct answer (7500).
# AI Use Log (3rd Use) 
- Tool/model & version: Gemini
- What I asked for: When working on problem 4, I was not sure how to go from odd to even in my specifications. 
- Snippet of prompt(s):
  Me: can you help me write a code to only read the even number of lines for practice.txt
  Gemini: Certainly! Here's a Python code snippet that will read the practice.txt file and print only the even-numbered lines.
This code opens the file, then iterates through each line using enumerate to get both the line number (starting from 0) and the line content.......
- What I changed before committing: I added the lines of code it suggested via hand typing them. I did not know about using enumerate and had planned on trying to just modify what I had practice typed in the 15.1 cell. So, I was glad to see a model of how the code needed to be to work. 
- How I verified correctness (tests, sample data): I used the test text from the Rosalind example before then using my code again with the generated problem #4 text. 
# AI Use Log (4th Use) 
- Tool/model & version: Gemini
- What I asked for: When i practiced 18.1 I could not understand if I was now in fasta or not, so I asked Gemini.
- Snippet of prompt(s):
  Me: is this code a fasfa file
  GeminiNo, the code in cell b-2XDof4rtP8 does not produce a FASTA file.
- What I changed before committing: I added the lines of code it suggested to make it a Fasta file (not graded part from Rosalind, I did this just for myself)
- How I verified correctness (tests, sample data): Tested for correctness and double checked it with the guide that it outputted how it was supposed to.
# AI Use Log (5th Use) 
- Tool/model & version: Gemini
- What I asked for: On the fifth Rosalind, I explained to Gemini what my goals were and it used the code I already had, tweaked it, and added a bit more that I then edited mine with its suggestions. 
- Snippet of prompt(s):
  Gemini: Excellent! You've got the right steps. Here's the code to implement the logic you described within a loop that reads from practice_5.txt.....
- What I changed before committing: I was messing up and realized it is because I was not using a text variable (I used a line variable). I changed it to text and also used gemini to work out the quirks in my loop over the words. 
- How I verified correctness (tests, sample data): Tested for correctness and used the practice set from Rosalind. 
# AI Use Log (6th Use) 
- Tool/model & version: Gemini
- What I asked for: When I ran my code from task 23.1 (modifying the code from 22.1) I got an import error. I asked Gemini to please explain the error. 
- Snippet of prompt(s):
  Gemini: The error in cell HsmdhYQOZe78, ImportError: cannot import name 'GC' from 'Bio.SeqUtils', indicates that Python couldn't find the name GC to import from the Bio.SeqUtils module.

While GC is indeed a function in Bio.SeqUtils,......

- What I changed before committing: I had to change when I imported GC, since it was currently importing inside the loop and not before it.  
- How I verified correctness (tests, sample data): Tested for correctness and used the practice set from Rosalind.
** This did not work ** Moved onto the Rosalind practice problem to try my luck with that. 
  6th use continued)
This still did not work and Gemini kept saying that GC was not the correct verbiage. I googled and found online that "gc_fraction" is the correct verbiage for the newer biopython models. So, I shifted it up and still had errors. I took a break from Gemini to see if chat GPT could explain it to me. That is when I realized I forgot it was still a txt file and I had left the parse/parameter line of code out from the example (still do not know if this was a correct fix?)
Then, I took the loop from chat gpt 
"for record in SeqIO.parse(filename, "fasta"):
        gc = gc_fraction(record.seq) * 100
        if gc > max_gc:
            max_gc = gc
            max_id = record.id" 

But I changed it to names that made sense to me and helped me udnerstand it better. (Did not just copy and paste without changing it and trying to internalize what it ws telling me) 
From there, I ran the code, there was some minor error (I think with indentation) that Gemini showed me. I fixed that, and then I verified correctness of my code using the Rosalind sample data. It finally worked, and I was so glad! 
