
### Json pros:
- easier for the computer to read
- Maybe less likely to get corrupted?
- Format preferred by APIs: I would learn skills for working with API data
- Allegedly more versatile, has more longevity - I have thoughts on this.
- Can deal with more complex data; graphs, networks, etc.
- Can be meaningfully combined with other data models 
- Shawn says it's better, and I trust Shawn
- An abstracted format might allow me to see my data "distantly"; find patterns that I otherwise wouldn't

### Json cons:
- Not intuitive for me; much steeper learning curve
- Average historian doesn't know how to derive meaning from a json file
- Hard to find beginner-friendly information about data querying and visualization
- I'm not sure how to check the data to make sure its right
- I don't have any "graph shaped questions" on my mind about the data

### CSV pros:
- Easier for me to read, more intuitive
- Average historian knows how to do something with a csv file, and how to make sense of the words in it
- The HBC account books are already in tabular format; csv would be like a digital analogue of the way 17th century accountants recorded their own data
- I can easily check my work. Source CSV files should have the same data in the same places as HBC accounts
- Can be visually represented 1:1
- Lots of beginner-friendly info out there for data visualization with CSVs
- I can imagine some relational database-shaped questions that would help my research vis a vis communicating things that I already have a sense of in data visualization
- Used in gov jobs

### CSV Cons
- Can't be easily combined with data in other models
- Less versatile; transmittable?
- Conflates container and content; usually used with proprietary software
- Not as easy for computer to read
- Not used for APIs



# What should I do?

I don't know anything about accounting other than what I've figured out just by looking at early modern account books a lot. To some extent, I want to do this project to validate my understanding of how these account books work. I want to really exercise my understanding of how the different values flow together, not so I can do cool digital data analytics, but so that I feel confident in the rest of my analysis of these documents. I am making a lot of assumptions about what the numbers mean, but if I make a relational database that is structured the way I think it should be and then the actual numbers get all jumbled, then I know I'm making some mistakes. 

If I make this data useable by other people, it has to be RIGHT, and this is more relevant the more useful the format is. Right now, I know one way to do this with csvs:  import CSV files into Google Sheets and manually compare them against the original pages in the records. I would like to automate corrections to the OCR, but having this way to check is really reassuring. I am sure there are ways to do this with json, but I would want to get to a point with it where I feel confident, and that seems like a huge project.

There is something there about the role of faith and abstraction in research. I've been trying to reckon with this in grad school a bit. I feel like I'm taking in so much information and I can kind of point to foucault or marx about something, but I don't really understand how they came to their ideas. I like knowing what I'm doing and what I'm thinking and how I'm coming to my conclusions on the level of actual human understanding. Getting really abstract with it is not that attractive to me. 

On a practical level, I found a really good looking beginner-friendly manual for the "tidyverse" package/package of packages, and it works with csv files. This takes out a lot of the guesswork of figuring out what will be compatible with what and just gives me a bunch of things to start playing with that I know will work together. I like the idea of having a csv file to reference that I really understand so that when I'm learning how to do freaky r things, I can actually see what is happening. 

The biggest downside to me of csv is that I wouldn't get to learn how to do stuff with json, and I am really intrigued by APIs, so that is a bummer. But I already have plenty of things to learn. So why not start with something that makes more sense to me.

# Data isn't real

Something that feels wrong about doing this in json is part of what's supposed to be good about it: the separation of content and container. The data in HBC accounts gets abstracted into something other than a clear account book. When I read an account book I know that I'm not looking at real shirts, I'm looking at the recorded number of shirts. I know that there was smuggling and errors and all kinds of stuff that might make this a bit different from reality. I know I'm looking at an hbc record of shirts, not just subjectivity-free data about real shirts.

I don't want this data to get treated as historical fact without the relevant contextual information. My whole practice is looking at this and being like "the word on the page means so much more than what is here." While json might open up some ways of linking account books with what is going on in letters, climate, wars, etc., the more data models you combine the less you understand the limitations and conditions of each of them. I want my research to be useable to other people, but a big part of my research is thinking about the gulf between record and reality, and that's squishy work.

I like thinking about this stuff because I'm generally on the side of more open research and open data. I didn't do a history undergrad, and got into grad school through the skills and knowledge I built through wikipedia, blogs, archive.org, etc.. So i'm into it!

It's not that I want to put a big barrier up between my work and other people using it, I just want to share what the important part of the work actually is: the squishy thinking about how these records need to be treated with a lot of grains of salt. Call me a papist, but I think often the learned discussion of the thing is more important to communicate than the thing, even when I'm communicating with other historians. 

This is probably reading to much into just the data format, but I feel like people love to just take data and mess around with it without understanding what the actual collection methods were and what the limitations of it are. This might be bad practice but it's common.

There is one very tangible example of how this could go wrong with fur trade accounts: there are all of these records of HBC goods being traded for x amount of beavers, but the beavers don't actually exist in these transactions. The beavers are imaginary accounting units. There are beaver pelts that come into the fort, but these are recorded separately from the imaginary beaver units that come in. The difference between imaginary beaver and real beaver is important and these two numbers are always different. (not worth explaining in depth here). 

What I'm describing here is not specific to json vs csv, but it points to the shape of what feels wrong. I think I like csv here because its preserving the structure of the 17th century container pretty darn well.

# Questions
- What is the difference between and excel file and a csv? What does excel/google sheets do to CSVs?
- Could I just work in CSV for simplicity and then put that stuff all in a json file for longevity's sake?

# Final thoughts

I know I'm overthinking this, and actually messing around with things is how I'm really going to figure out what works, but this was a good exercise in mapping out some sketchy thoughts.

I think I'm going to go forward with CSVs first since I know where to start, and then if I have time I'll try to replicate some of what I do with json. 
