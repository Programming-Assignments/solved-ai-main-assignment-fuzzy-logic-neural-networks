Download Link: https://assignmentchef.com/product/solved-ai-main-assignment-fuzzy-logic-neural-networks
<br>
You are required to use <strong><em>fuzzy logic</em></strong>, <strong><em>neural networks</em></strong> AI technologies to control a set of characters that are moving randomly through a game model. The AI controlled characters should be able to interact both with each other and the single instance of a user-controlled player. A suite of stubs is provided on Moodle that already implements a JavaFX game window with a model, view and controller. A thread pool containing a set of runnable autonomous characters has also been implemented already.




The purpose of this assignment is for you not to programme a game, but to <strong><em>design and implement fuzzy logic and neural network controllers for the autonomous game characters</em></strong>. Therefore, much of the programming will be declarative, e.g. fuzzy control language or involve secondary AI design considerations such as developing a neural network topology or preparing, transforming and processing training data. You have been given an <strong><em><u>open brief</u></em></strong> regarding the function and nature of interaction of the different game characters and you are free to implement any reasonable behaviour that you see fit. This extends to the actual goal of the game and how the game should terminate. Consequently, will have to <strong><em><u>carefully document your rationale</u></em></strong> for each of the design decisions that you make and justify the various approaches that you have employed.







<h1>Minimum Requirements</h1>

<ul>

 <li>Clearly <strong><em><u>document</u></em></strong> in a README file the overall goal for the game and your rationale for the set of controllers that you have implemented. You must document all aspects of the fuzzy controller(s) that you design, as well as the architecture, activation functions and input vectors to your neural network. Any hyperparameters should be clearly reasoned and presented.</li>

 <li>Only use the <strong><em>JFuzzyLogic</em></strong> and <strong><em>Encog 3.4</em></strong> Do not use any other 3<sup>rd</sup> party software. You can asset-strip, repackage and re-use any of the code from the AI labs, including the 3-layer neural network.</li>

 <li>Each character should be <strong><em>controlled by some intelligence</em></strong>, either fuzzy logic, a neural network, a heuristically informed search algorithm or even a cocktail of all three.</li>

 <li>The fuzzy logic should be encapsulated in one of more FCL files and placed in a <strong>./<em>resources/fuzzy</em></strong> You should consider carefully the following when designing the fuzzy logic components of the system:</li>

</ul>




<ul>

 <li><strong>Linguistic variables</strong> and Universe of Discourse</li>

 <li><strong>Fuzzy Sets</strong> and Membership Functions</li>

 <li><strong>Defuzzifiers</strong>, e.g. COG, COGS, LM, MM, RM.</li>

 <li>Membership Functions for output variables, e.g. <strong>Mamdani</strong> or <strong>Suegno</strong>.</li>

 <li><strong>Fuzzy Rules</strong>. All fuzzy sets must be covered by at least one fuzzy rule.</li>

</ul>




You must <strong><em><u>comment the FCL with your rationale</u></em></strong> for each of the design decisions that you make. Note that you can include more than one function block per FCL file.




<ul>

 <li>The neural network should be trained, in a reasonable amount of time (&lt; 1 minute), when the game starts up and have a <strong>fully documented topology</strong> presented in the README. Do not use any other 3<sup>rd</sup> party implementation. All the training and validation resources for the neural network should be placed in the <strong>./<em>resources/neural</em></strong></li>

</ul>




<ul>

 <li>You can assume that the <strong>JavaFX</strong> library and the dependencies for <strong>Encog 3.4</strong> and the <strong>JFuzzyLogic</strong> libraries are already available on the <strong><em>module-path</em></strong>. These have already been added to the <strong><em>module-info.java</em></strong> module descriptor. Do not include any of these dependencies with your submission or change how they are declared in the module descriptor.</li>

</ul>







<h1>Deployment and Delivery</h1>

Please <strong>read the following carefully</strong> and pay particular attention to the files that you are required to submit and those that you should not include with your assignment:

<ul>

 <li><strong><em>The project must be submitted by midnight on Sunday 4<sup>th</sup> April 2021</em></strong>. Before submitting the assignment, you should review and test it from a command prompt on <strong><em><u>a different computer</u></em></strong> to the one that you used to program the project.</li>

 <li>The project must be submitted as a Zip archive <strong><em>(not a 7z, rar or WinRar file)</em></strong> using the Moodle upload utility. You can find the area to upload the project under the “<em>Autonomous Computer-controlled Game Characters – (50%) Assignment Upload</em>” link on Moodle. Only the contents of the submitted Zip will be considered. <strong><em><u>Do not add</u></em></strong><strong><em> <u>comments to the Moodle assignment upload form.</u></em> </strong></li>

 <li>The name of the Zip archive should be <em>&lt;id&gt;</em>.zip where<em> &lt;id&gt;</em> is your GMIT student number.</li>

 <li>The Zip archive should have the structure shown below. Do NOT submit the assignment as an Eclipse project.</li>

</ul>




<table width="550">

 <tbody>

  <tr>

   <td width="106"><strong>Marks </strong></td>

   <td width="444"><strong>Category </strong></td>

  </tr>

  <tr>

   <td width="106"><strong>game.jar</strong></td>

   <td width="444">A Java archive containing your API and runner class with a <strong><em>main()</em></strong> method. You can create the JAR file using the following command from inside the “<strong>bin</strong>” folder of the Eclipse project: <strong>jar -cf game.jar * </strong> The application should be executable from a command line using the <strong>module-path</strong> as follows: •       <strong><u>Linux/Mac:</u></strong> <strong>java </strong><strong>–module-path</strong><strong> .:/path/to/your/javafx-sdk-</strong><strong>11.                 </strong><strong>0.2/lib:/path/to/your/encog-3.4/:/path/to/your/jfuzzylogic </strong><strong>–module </strong><strong>gmit.software/ie.gmit.sw.ai.Runner</strong> •       <strong><u>Windows:</u></strong> <strong>java </strong><strong>–module-path</strong><strong> .</strong><strong>;</strong><strong>/path/to/your/javafx-sdk-</strong><strong>11.                 </strong><strong>0.2/lib</strong><strong>;</strong><strong>/path/to/your/encog-3.4/</strong><strong>;</strong><strong>/path/to/your/jfuzzylogic </strong><strong>–module </strong><strong>gmit.software/ie.gmit.sw.ai.Runner</strong> You only need to use the module-path syntax above to check your application after creating the JAR. Change the parameter /path/to/your/ to the real system path on your computer.</td>

  </tr>

  <tr>

   <td width="106"><strong>resources</strong></td>

   <td width="444">A directory that contains <strong>all the resources</strong> required by the application. You can add to the existing set of subdirectories (<em>images, fuzzy, neural</em>) if necessary. All fuzzy</td>

  </tr>

  <tr>

   <td width="106"> </td>

   <td width="444">definitions should be stored in the <strong><em>fuzzy</em></strong> directory and neural network training and validation data in the <strong><em>neural</em></strong> directory.</td>

  </tr>

  <tr>

   <td width="106"><strong>src </strong></td>

   <td width="444">A directory that contains the packaged <strong>source code</strong> for your application.</td>

  </tr>

  <tr>

   <td width="106"><strong>README.pdf </strong></td>

   <td width="444">A <strong>PDF</strong> file detailing the main features of your application in <strong><u>no more than 300 words</u></strong>. All <strong>features and their design rationale</strong> must be fully documented.</td>

  </tr>

 </tbody>

</table>