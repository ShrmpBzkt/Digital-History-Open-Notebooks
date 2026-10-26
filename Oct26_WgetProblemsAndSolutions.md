I made some notes on problems I had as I did some of Kurschinski's Applied Archival Downloading with wget tutorial.
Maybe these will be helpful to anyone else who runs into problems
I did it in colab because I don't have anything set up to run python on my computer, and also that means you can do it even if you're having trouble installing wget on your computer.

Also, hot github tip, you can end your file names with .md to make them look like this instead of plain text.


# Recursive Retrieval and Sequential URLs

- Problem: the tutorial doesn't explain how to run python code. 
	- Run the code from colab
- Problem: I forget how to save files from colab
	- solution: you can see the working directory on the side bar. I'm sure there are other ways but this is helpful.
- Problem: errors galore when I run the code
	- solution: I forgot to replace the integer placeholders with actual numbers oopsies
- Problem: my urls.txt file just says "1"
	- Had to add () after close function: f.close()
		- solved! got my file
- Problem: what is the -i option for wget?
	- it is for files
- ran this code in collab:
	- ! wget -i urls.txt --limit-rate=100k -w 1 -np -nd
	- seems successful. Files downloaded to colab directory. Could probably run code minus ! in command line and get the same results on OS (assuming wget is succesfully installed)
		- You don't need to install wget in colab, just use the bash ! command
- Comment: None of this uses the -r option. Why is this called recursive retrieval?

- the next two examples were pretty straightforward, so I skipped them
# More Complicated Recursive Retrieval: A Python Script for Leading Zeros
- This is the exact situation of the Hudsons Bay Company Archives that I want to download from (leading zeros and a closed directory). So I'm excited to try this.
- Not gonna actually download these bad boys, just run the python code to get a file of the urls, that I could use wget -i on
- had to do f.close() again
- success! got a txt file with the URLs
