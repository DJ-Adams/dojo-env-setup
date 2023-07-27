# dojo-env-setup

<img src="images/Data Science Thumbnail.png">

- **If you are looking for the original dojo-env environment from pre-July 2022**, switch to the legacy-dojo-env-v1 branch after cloning this repository. 
<img src="images/legacy-branch.png" width=400px>

<!DOCTYPE html>
<html><body><h1>Installing Python Locally</h1><br><hr></hr><br><div id="lesson_content">
 <h1>
  Installation Overview
 </h1>
 <p>
  So far in this program, you have been working in Google Colab which provides a cloud-based coding environment.  We will be transitioning to using a Python environment stored on your local machine.  You will be working in Jupyter Notebook, which is very common in the data industry.  In addition, these instructions will include the installation of Github Desktop and Visual Studio Code (VS Code).
 </p>
 <ul>
  <li>
   In the Advanced Machine Learning course, you will need to submit a
   <strong>
    CORE ASSIGNMENT
   </strong>
   containing the error-free test notebook that is included within these instructions.  This will ensure that you have the tools you will need to be successful.
  </li>
 </ul>
 <ul>
  <li>
   We recommend you begin the step-by-step installation
   <strong>
    AS SOON AS POSSIBLE
   </strong>
   to ensure you have time to troubleshoot any difficulties you may encounter.
  </li>
 </ul>
 <ul>
  <li>
   If you run into issues during installation, post your questions/issues on the
   <a href="https://discord.com/channels/738494436467539968/999108307627294770" target="_blank">
    ds-python-installation
   </a>
   Discord channel, and tag your instructor in your question (e.g. @dojo_Instructor_name).
  </li>
 </ul>
 <ul>
  <li>
   <strong>
    These steps should take  ~30-90 minutes,
   </strong>
   depending on the speed of your machine and internet connection.
  </li>
 </ul>
 <ul>
  <li>
   The
   <a href="https://github.com/coding-dojo-data-science/dojo-env-setup" target="_blank">
    dojo-env-setup repository
   </a>
   , which you will clone in Step 2.1, contains a backup copy of the entire set of instructions on the README, for convenience.
  </li>
 </ul>
 <hr/>
 <blockquote>
  Note: if you previously installed the dojo-env and are upgrading to the current version, please see the "Updating to New dojo-env" at the end of this chapter (after the Final Notes lesson)
 </blockquote>
 <p>
  <strong>
   By the end of this chapter, you will:
  </strong>
 </p>
 <ol>
  <li>
   Install GitHub Desktop,
  </li>
  <li>
   Install Python via Anaconda (or via miniforge - if on a Mac with an Apple Chip)
  </li>
  <li>
   Create a special Python environment (dojo-env)
  </li>
  <li>
   Supercharge Jupyter Notebooks with Extensions
  </li>
  <li>
   Install Visual Studio Code.
  </li>
 </ol>
 <h2>
  If you encounter an error during installation:
 </h2>
 <ul>
  <li>
   <strong>
    First, read a little further down in the instructions to make sure we do not already address
   </strong>
   the error message that you ran into.
  </li>
  <li>
   Second,
   <strong>
    please check the "Troubleshooting" chapter
   </strong>
   for a lesson about the problem you are running into.
   <br/>
   (The Troubleshooting section is the 3rd chapter in this course - see the screenshot below)
   <p>
    <br/>
   </p>
   <figure>
    <img height="193" src="images/lp/Troubleshooting-chapter.png" style="width: 191px; height: 193px;" width="191"/>
   </figure>
  </li>
  <li>
   Third, reach out on the #ds-python-installation Discord channel (
   <a href="https://discord.com/channels/738494436467539968/999108307627294770" target="_blank">
    Link
   </a>
   ) with:
   <ul>
    <li>
     What step you are on (e.g. Step 2.3 Creating the dojo-env)
    </li>
    <li>
     What OS you are using (e.g. Windows 10, Windows 11, Mac with an Apple Processor, etc)
    </li>
    <li>
     Screenshots of the error/issue you are running into, whenever possible.
    </li>
    <li>
     Finally, if you have been able to run the test notebook in Step 2.4: Testing the Env, please upload these files with your question.
    </li>
   </ul>
  </li>
  <li>
   Fourth, if you do not receive a response by the end of the day on Discord, please email your instructor.
  </li>
 </ul>
 <hr/>
 <h2>
  OS-Specific Steps/Commands
 </h2>
 <p>
  <strong>
   For several steps (e.g. Step 1), there are multiple versions of the instructions, depending on what operating system you are using.
  </strong>
 </p>
 <p>
  (i.e. a Windows computer, vs a Mac with an Intel processor, vs a Mac with an Apple Chip (m1/m1pro/m2/etc).)
 </p>
 <p>
  <dfn>
   For step 1, please make sure you are on the correct instruction page for your OS.
  </dfn>
 </p>
 <h3>
  Currently Supported Operating Systems
 </h3>
 <ul>
  <li>
   We have prepared environment files (.yml files) for 4 different OS configurations:
   <ul>
    <li>
     Windows (10 &amp; 11)
    </li>
    <li>
     Mac (with Intel processors)*
    </li>
    <li>
     Mac (Apple Chips)*
    </li>
    <li>
     Linux**
    </li>
   </ul>
  </li>
 </ul>
 <h4>
  *Note for Mac users - if you don't know which type of Mac you have :
 </h4>
 <div>
  <ul>
   <li>
    Check the "About this Mac" screen for your computer.
    <ul>
     <li>
      Click on the Apple symbol on the top-left corner of your screen.
     </li>
     <li>
      <strong>
       Click About This Mac.
      </strong>
     </li>
     <li>
      A window with your computer's specs will appear like the one in the screenshot below
      <ul>
       <li>
        <img height="268" src="images/lp/About_this_Mac_-Intel.png" style="background-color: initial; width: 475px; height: 268px;" width="475"/>
       </li>
      </ul>
     </li>
     <li>
      If it has a "Processor" line that says "Intel" you should follow the Instructions: Mac (Intel Processor).
     </li>
     <li>
      If it has a "Chip" line that says "Apple" then you should follow the Instructions: Mac (Apple Chip).
     </li>
    </ul>
   </li>
  </ul>
  <h4>
   **Note to Linux Users:
  </h4>
  <ul>
   <li>
    Our Linux installation instructions are still in beta. While they have successfully been installed on students' Linux machines, we currently do not have a Linux machine available for troubleshooting.
    <ul>
     <li>
      The beta Linux instructions are located
      <a href="https://login.codingdojo.com/m/213/13909/99742" target="_blank">
       here
      </a>
      and all steps are combined into 1 lesson.
     </li>
    </ul>
   </li>
  </ul>
  <p>
   <br/>
  </p>
  <hr/>
  <p>
   <strong>
    Regardless of OS, you will be using tools that serve the following purposes:
    <br/>
   </strong>
  </p>
  <ul>
   <li>
    Your "Terminal"/"Shell":
    <ul>
     <li>
      The primary application you will use to execute coding-related commands.
     </li>
    </ul>
   </li>
   <li>
    A Python Distribution:
    <ul>
     <li>
      The fundamental infrastructure for installing Python.
     </li>
    </ul>
   </li>
   <li>
    GitHub Desktop:
    <ul>
     <li>
      App for working with and managing git repositories.
     </li>
    </ul>
   </li>
   <li>
    Our custom Python Environment (dojo-env)
    <ul>
     <li>
      A bundle of packages required for stacks 1-5+
     </li>
    </ul>
   </li>
   <li>
    Jupyter Notebooks / Jupyter Lab
    <ul>
     <li>
      The primary editor we will use (instead of Colab).
     </li>
    </ul>
   </li>
   <li>
    Visual Studio Code
    <ul>
     <li>
      A special text editor designed for code. It has many extensions and languages available.
     </li>
     <li>
      We will use it to edit special files, but it can also run notebooks too!
     </li>
    </ul>
   </li>
  </ul>
  <hr/>
  
  <hr><hr>


## Instructions 
- [Windows](./docs/instructions-windows-v23.md)
- [Mac-Apple Chip (m1,m2,etc.)](./docs/instructions-mac-mchip-v23.md)
- [Mac-Intel](./docs/instructions-mac-intel-v23.md)
- `WIP` Linux[]]()