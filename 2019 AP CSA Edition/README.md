# 2019 Advanced Placement Computer Science A Edition
Notes and Progressions for CSA

**UNDER CONSTRUCTION**

## Progressions
- Reminder: routines in the course for each week
- Barron's in Order: Ch 3, Ch 1, etc. (~3 weeks allowing for CSP Introduction and Teacher Directed Instruction)
- Complete Labs, See Below in To Include until Section is Created (~two weeks per lab, while CSP works on conceptual and translation work)

## Routines throughout the Course

### Vocabulary Development

Tuesday and Thursday Vocabulary Development
- **Purpose**: answer "How do we write about the programs we are supposed to use (CSP)", and, "How do we read the exam (CSA)"
- Where have we seen these words or concepts before (previous projects, current project)
- How do we include other words we need to include that we personally have trouble with

### Using Barron's Computer Science A Resources, Flash Cards

Wednesday and Friday Flash Card Questions and Review
- **Purpose**: review all flash cards twice through the semester
- Read flash questions so students need to work for understanding (never before has evaluation happened like this, usually only project-based), read only twice for students to generate first answer
  - max time: 90 seconds for reading and answer
- Use Document Camera to post flash cards after all flash cards read

Additional Resources used as "Wednesday-Friday Questions"
- True False Questions
- Writing Statement Prompts
- Calculation Questions, see Barron's Flash Cards
  - All levels, General Trivia
  - All levels, Number Conversions
  - CS10: Arithmetic Statements, Relational Statements, Compound Statements
  - CS10: Integer Class Search Functions (max & min values, random, etc.)
  - CS10: FOR & WHILE LOOPS, including Nested FOR (number of execution times, variable skip-counting)
  - CS20: Array Questions
  - CS30: String Functions
  - CS30: `compare.To` Questions
  - CS30: Search Algorithm Comparison Questions
- Summary of all Cue Cards, Algorithm Analysis (only done in AP CS 35)

Add to these a list of "Describe these Functions", seen in CS10, CS20, and CS30 (Pure Java)

---

## Resources to Include in the Above Progression (<a href="">Jump to the Progressions Above</a>)
  - Interactive Java Review, <a href="http://interactivepython.org/runestone/static/JavaReview/index.html">Click Here</a>
    - Advice: start with Practice Exams, review the sections needing review

---

# Ideas to Include

Explore https://edhesive.com/courses/apcs_java (Code.org CSA)

---

- Labs
  - Chatbot, Processing.org (machine learning? using Chatbot from "How to think like a Computer Scientist, stringdict as key-value pairs with hash-separations, Exact Match, Phrase Match, Word Match, Random Match, "I like ... (apples), "I like (apples) too", need to write items to a file and read it back)
  - See Notes from CS Symposium
  - See <a href="https://drive.google.com/drive/folders/1C2pq0Csfiyf5f3neOdoDBJxmRQMeYlt3">Mr. Mercer Teacher Only Files</a>
  - Special Thank-you to Janice Parsons, see <a href="https://drive.google.com/drive/folders/18vIwVZfKiE2DL1J5Wt3sWVXPxRBJVdNl">Publically Shared Folder</a>
  - Solitare using Greenfoot (you play, and if you write it well will play itself in 5 lines of code)
  - <a href="https://drive.google.com/drive/folders/1IMoqA7wAUiNJA7rKvISg3RQ472mAiSiy">Example Solitare Lab</a>
  - Pictures Lab uses Eclispe

Chatbot Labs


- <a href="https://drive.google.com/drive/folders/18vIwVZfKiE2DL1J5Wt3sWVXPxRBJVdNl">Janice's Chatbot Files</a>
- Google Search Parts of the Labs
- Chatbot
  - <a href="https://www.google.com/search?q=StringExplorer+ap+csa&rlz=1C1GCEA_enCA818CA818&oq=StringExplorer+ap+csa+&aqs=chrome..69i57.4285j0j7&sourceid=chrome&ie=UTF-8">StringExplorer ap csa</a>
  - <a href=""></a>
---

Chatbot Progressions
- <a href="https://apstudent.collegeboard.org/apcourse/ap-computer-science-a/course-details/lab-requirements">Student Lab Links</a>
- - http://media.collegeboard.com/digitalServices/pdf/ap/ap-compscia-magpie-lab-student-guide.pdf
- Introduction: focusing on String Method and IF Statements
- [Optional] Activity 1: Getting Acquainted with Chatbots: <a href="https://chatbots.org/">Explore this Website, Chatbots.org</a>
  - <a href="https://sites.google.com/site/webtoolsbox/bots">Alternate Website, Webtools for Kids</a>
  - <a href="https://www.cleverbot.com/">Cleverbot</a>
  - Try out several chatbots by trying several conversations
  - Explore with some difficult questions like (i.e. try to find the bugs)
    - "Where do you come from?"
    - "Who are you?"
    - "How are you?"
    - What are you?"
  - Explore other questions to find ...
    - What is the most interesting response?
    - What is the most peculiar response?
    - How does it respond to “asdfghjkl;”?
  - Summary Questions to answer to help develop your own chatbot
  - Simple chatbots act by looking for keywords or phrases and responding to them.
    1.	Identify keywords to which your chatbot responds?
    2.	Does it learn from your responses?  How do you know?
    3.	How many different responses to the same question before you get repeats?
    4.	Is the chatbot using the history of the conversation to guide its answers?
- Activity 2: Introduction to the Magpie Class
  -

---

We start with the translation program. Read in children's stories -- output a translation.
and the getWords - which is this case was French. (We just put our word list into Google translate)

Then the chatbot file has the code I worked through with the kids in class.
There are commented out lines where we changed how we did it.  Play with it. Let me know if you have any questions.

---

```Java
//FileReading.txt
String [] lines;
String [] words;
StringList newWords;

void setup() {
  lines = loadStrings("gingerbread.txt");
  println(lines.length);
  newWords = new StringList();
  for (int i=0; i<lines.length; i++)
  {
    words = splitTokens(lines[i], " ,.?\"");
    for (int j=0; j<words.length; j++)
    {
      if (!newWords.hasValue(words[j]))
        newWords.append(words[j]);
    }
  }
  println(newWords, newWords.size());
}
```
