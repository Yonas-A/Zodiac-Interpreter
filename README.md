 
# Astrological Divergence: Truest Zodiac Sign
 
 > Authors:
\<[Omar Hernandez](http//github.com/ohern017)\>
\<[Shamarri Coleman](https://github.com/sham-745)\>
\<[Yonas Adamu](https://github.com/Yonas-A)\>
 

## Project Description

 > * Why is it important or interesting to you?
 >   * It is very easy for one to find their own zodiac sign. No surprises here; all it takes for one to know what their zodiac sign is to know their birthday and find zodiac sign that corresponds to it. However, how well does it define you? That's the question we want ask with this program. What this program will do is quiz the user on their personality and determine what zodiac sign they match the most according to their answers. The program will also contrast the user's zodiac sign with what they got in the quiz, perhaps to raise questions as to the veracity of the very concept itself.
 > * What languages/tools/technologies do you plan to use?
 >   * We plan to use C++ for this project.
 > * What will be the input/output of your project?
 >   * The inputs of the project will be the user’s birthday and their quiz responses. The output will be the zodiac sign they get according to the answers they’ve provided to the quiz and also what their zodiac sign is according to their birthday. A further development goal that can be pursued here is an analysis of the contrasts as an additional output.
> * What are the three design patterns you will be using?
 >   1)  **Composite**:
The zodiac signs will create a hierarchical structure that appears to be appropriate for the Composite pattern. In addition to that, since the ultimate goal of the program is to output zodiac signs, the elements will really only serve as useful abstract classes that the concrete classes, such as the zodiac signs, will inherit the bulk of their information
 >   2)  **Facade**:
The zodiac signs will contain a number of characteristics that are common with the zodiac signs. After retrieving the characteristics from their superclasses, the zodiac sign class will include the information that sets the specific zodiac sign apart from those of the same element. For this reason, it is believed that the Factory Method design pattern will be a good fit.
 >   3)  **Mediator**:
Since the user will be matched with potentially two different zodiac signs, a comparison between the two signs should be considered. Furthermore, for a deeper analysis, there may need to be interaction between the classes to further emphasize points of deviation. For this reason, we want to promote loose coupling so that deeper comparisons/analysis can be done.

 > ## Phase II
 
## Class Diagram
 > ![zodiac final project](https://user-images.githubusercontent.com/72321122/99348285-17fdc800-284e-11eb-8ac4-8cbecc7dc3e9.png)
 >
 
 >Composite:
The inputs from the client into the Date class are taken into the ActualZodiac class, where a zodiac sign is determined according to the user's birthday. Afterwards, the birthday zodiac sign is compared to the quiz zodiac sign via the compareZodiac function to eventually illustrate the depth of the contrast to the user. The resulting zodiac signs will be output by the displayZodiac function.

 >Mediator: 
Client input into Quiz class will be stored within arrays in the Score class. The highest score is then determined by the calculateScore function. The Zodiac class will determine which element class has the highest score from getTotalScore function. The appropriate zodiac will be output by the displayZodiac function based on the total score. 

 >Facade:
The Quiz class provides an interface to the user and walks them through the entire process without needing for the client to communicate with the questions class. The Quiz class is the composition of all of the questions, allowing for different types of questions grouped together while also making it easy to move through the questions themselves.

 > ## Phase III

 > ## Final deliverable
 >
 ## Screenshots
 > ![zodiacoutput1](https://user-images.githubusercontent.com/72321122/101879259-e8d53080-3b45-11eb-9421-269c21e1fdb9.png)
 >
 
 ## Installation/Usage
 > Enter your birthdate in number format (month, day, year). Then, take the Zodiac quiz by answering the 12 multiple choice questions. The answer choices are to be entered as 'a, b, c, or d' for each question. After completing the Zodiac quiz, you will receive a message containing your actual birth zodiac and the one determined by the Zodiac quiz along with some attributes associated with each zodiac sign.
 
 ## Testing
 >Unit-tested using google tests for each class.
 
