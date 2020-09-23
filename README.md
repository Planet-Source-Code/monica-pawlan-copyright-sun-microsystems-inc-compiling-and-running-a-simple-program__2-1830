<div align="center">

## Compiling and Running A Simple Program


</div>

### Description

This lesson explains how to write, compile, and run a simple program written in the Java TM language (Java program) that tells your computer to print a one-line string of text on the console.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Monica Pawlan \(Copyright Sun Microsystems Inc\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/monica-pawlan-copyright-sun-microsystems-inc.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |Java \(JDK 1\.1\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/monica-pawlan-copyright-sun-microsystems-inc-compiling-and-running-a-simple-program__2-1830/archive/master.zip)





### Source Code

<table border="0" cellPadding="0" cellSpacing="0">
 <tbody>
  <tr>
   <td>
    <table>
     <tbody>
      <tr>
       <td vAlign="top">
        <p><font face="Verdana">The computer age is here to stay.
        Households and businesses all over the world use computers in
        one way or another because computers help individuals and
        businesses perform a wide range of tasks with speed, accuracy,
        and efficiency. Computers can perform all kinds of tasks ranging
        from running an animated 3D graphics application with background
        sound to calculating the number of vacation days you have coming
        to handling the payroll for a Fortune 500 company.</font>
        <p><font face="Verdana">When you want a computer to perform
        tasks, you write a program. A program is a sequence of
        instructions that define tasks for the computer to execute. This
        lesson explains how to write, compile, and run a simple program
        written in the Java<font size="-2"><sup>TM</sup></font> language
        (Java program) that tells your computer to print a one-line
        string of text on the console.</font>
        <p><font face="Verdana">But before you can write and compile
        programs, you need to understand what the Java platform is, and
        set your computer up to run the programs.</font>
        <ul>
         <li><a href="#platform"><font face="Verdana">A Word About the
          Java Platform</font></a>
         <li><a href="#setup"><font face="Verdana">Setting Up Your
          Computer</font></a>
         <li><a href="#simple"><font face="Verdana">Writing a Program</font></a>
         <li><a href="#comp"><font face="Verdana">Compiling the Program</font></a>
         <li><a href="#run"><font face="Verdana">Interpreting and
          Running the Program</font></a>
         <li><a href="#debug"><font face="Verdana">Common Compiler and
          Interpreter Problems</font></a>
         <li><a href="#comm"><font face="Verdana">Code Comments</font></a>
         <li><a href="#api"><font face="Verdana">API Documentation</font></a>
         <li><a href="#more"><font face="Verdana">More Information</font></a></li>
        </ul>
        <font face="Verdana, Arial, Helvetica, sans-serif">
        <hr>
        <a name="platform"></a></font>
        <h3><font face="Verdana">A Word About the Java Platform</font></h3>
        <font face="Verdana">The Java platform consists of the Java
        application programming interfaces (APIs) and the Java<a href="#TJVM"><sup>1</sup></a>
        virtual machine (JVM).</font>
        <p><font face="Verdana"><img align="left" src="http://www.planet-source-code.com/vb/tutorial/java/images/platform.gif" >
        Java APIs are libraries of compiled code that you can use in
        your programs. They let you add ready-made and customizable
        functionality to save you programming time.</font>
        <p><font face="Verdana">The simple program in this lesson uses a
        Java API to print a line of text to the console. The console
        printing capability is provided in the API ready for you to use;
        you supply the text to be printed.</font>
        <p><font face="Verdana">Java programs are run (or interpreted)
        by another program called the Java VM. If you are familiar with
        Visual Basic or another interpreted language, this concept is
        probably familiar to you. Rather than running directly on the
        native operating system, the program is interpreted by the Java
        VM for the native operating system. This means that any computer
        system with the Java VM installed can run Java programs
        regardless of the computer system on which the applications were
        originally developed.</font>
        <p><font face="Verdana">For example, a Java program developed on
        a Personal Computer (PC) with the Windows NT operating system
        should run equally well without modification on a Sun Ultra
        workstation with the Solaris operating system, and vice versa. <a name="setup"></a></font>
        <h3><font face="Verdana">Setting Up Your Computer</font></h3>
        <font face="Verdana">Before you can write and run the simple
        Java program in this lesson, you need to install the Java
        platform on your computer system.</font>
        <p><font face="Verdana">The Java platform is available free of
        charge from the <a href="http://java.sun.com/products/jdk/1.2/" target="_blank">java.sun.com</a>
        web site. You can choose between the Java® 2 Platform software
        for Windows 95/98/NT or for Solaris. The download page contains
        the information you need to install and configure the Java
        platform for writing and running Java programs.</font><font face="Verdana, Arial, Helvetica, sans-serif">
        <p>&nbsp;
        <blockquote>
         <hr>
        </font><font face="Verdana"><strong>Note:</strong> Make sure you
        have the Java platform installed and configured for your system
        before you try to write and run the simple program presented
        next.</font><font face="Verdana, Arial, Helvetica, sans-serif">
        <hr>
        </blockquote>
        <a name="simple"></a></font>
        <h3><font face="Verdana">Writing a Program</font></h3>
        <font face="Verdana">The easiest way to write a simple program
        is with a text editor. So, using the text editor of your choice,
        create a text file with the following text, and be sure to name
        the text file <code>ExampleProgram.java</code>. Java programs
        are case sensitive, so if you type the code in yourself, pay
        particular attention to the capitalization.</font>
        <pre><font face="Verdana">//A Very Simple Example
class ExampleProgram {
 public static void main(String[] args){
  System.out.println(&quot;I'm a Simple Program&quot;);
 }
}
</font></pre>
        <font face="Verdana">Here is the <a href="http://www.planet-source-code.com/vb/tutorial/java/samples/ExampleProgram.java">ExampleProgram.java</a>
        source code file if you do not want to type the program text in
        yourself. <a name="comp"></a></font>
        <h3><font face="Verdana">Compiling the Program</font></h3>
        <font face="Verdana">A program has to be converted to a form the
        Java VM can understand so any computer with a Java VM can
        interpret and run the program. Compiling a Java program means
        taking the programmer-readable text in your program file (also
        called source code) and converting it to bytecodes, which are
        platform-independent instructions for the Java VM.</font>
        <p><font face="Verdana">The Java compiler is invoked at the
        command line on Unix and DOS shell operating systems as follows:</font>
        <pre><font face="Verdana"> javac ExampleProgram.java
</font></pre>
        <font face="Verdana, Arial, Helvetica, sans-serif">
        <blockquote>
         <hr>
        </font><font face="Verdana"><strong>Note:</strong> Part of the
        configuration process for setting up the Java platform is
        setting the class path. The class path can be set using either
        the <code>-classpath</code> option with the <code>javac</code>
        compiler command and <code>java</code> interpreter command, or
        by setting the <code>CLASSPATH</code> environment variable. You
        need to set the class path to point to the directory where the <code>ExampleProgram</code>
        class is so the compiler and interpreter commands can find it.
        See <a href="http://java.sun.com/products/jdk/1.2/docs/tooldocs/tools.html" target="_blank">Java
        2 SDK Tools</a> for more information.</font><font face="Verdana, Arial, Helvetica, sans-serif">
        <hr>
        </blockquote>
        <a name="run"></a></font>
        <h3><font face="Verdana">Interpreting and Running the Program</font></h3>
        <font face="Verdana">Once your program successfully compiles
        into Java bytecodes, you can interpret and run applications on
        any Java VM, or interpret and run applets in any Web browser
        with a Java VM built in such as Netscape or Internet Explorer.
        Interpreting and running a Java program means invoking the Java
        VM byte code interpreter, which converts the Java byte codes to
        platform-dependent machine codes so your computer can understand
        and run the program.</font>
        <p><font face="Verdana">The Java interpreter is invoked at the
        command line on Unix and DOS shell operating systems as follows:</font>
        <pre><font face="Verdana"> java ExampleProgram
</font></pre>
        <font face="Verdana">At the command line, you should see:</font>
        <pre><font face="Verdana"> I'm a Simple Program
</font></pre>
        <font face="Verdana">Here is how the entire sequence looks in a
        terminal window:</font>
        <p><font face="Verdana"><img src="http://www.planet-source-code.com/vb/tutorial/java/images/examprog.gif"></font>
        <p>&nbsp;
        <h3><font face="Verdana">Common Compiler and Interpreter
        Problems</font></h3>
        <font face="Verdana">If you have trouble compiling or running
        the simple example in this lesson, refer to the <a href="http://java.sun.com/docs/books/tutorial/getStarted/problems/index.html" target="_blank">Common
        Compiler and Interpreter Problems</a> lesson in <a href="http://java.sun.com/docs/books/tutorial/trailmap.html" target="_blank">The
        Java Tutorial</a> for troubleshooting help. <a name="comm"></a></font>
        <h3><font face="Verdana">Code Comments</font></h3>
        <font face="Verdana">Code comments are placed in source files to
        describe what is happening in the code to someone who might be
        reading the file, to comment-out lines of code to isolate the
        source of a problem for debugging purposes, or to generate API
        documentation. To these ends, the Java language supports three
        kinds of comments: double slashes, C-style, and doc comments.</font>
        <h4><font face="Verdana">Double Slashes</font></h4>
        <font face="Verdana">Double slashes (<code>//</code>) are used
        in the C++ programming language, and tell the compiler to treat
        everything from the slashes to the end of the line as text.</font>
        <pre><font face="Verdana">//A Very Simple Example
class ExampleProgram {
 public static void main(String[] args){
  System.out.println(&quot;I'm a Simple Program&quot;);
 }
}
</font></pre>
        <h4><font face="Verdana">C-Style Comments</font></h4>
        <font face="Verdana">Instead of double slashes, you can use
        C-style comments (<code>/* */</code>) to enclose one or more
        lines of code to be treated as text.</font>
        <pre><font face="Verdana">/* These are
C-style comments
*/
class ExampleProgram {
 public static void main(String[] args){
  System.out.println(&quot;I'm a Simple Program&quot;);
 }
}
</font></pre>
        <h4><font face="Verdana">Doc Comments</font></h4>
        <font face="Verdana">To generate documentation for your program,
        use the doc comments (<code>/** */</code>) to enclose lines of
        text for the <code>javadoc</code> tool to find. The <code>javadoc</code>
        tool locates the doc comments embedded in source files and uses
        those comments to generate API documentation.</font>
        <pre><font face="Verdana">/** This class displays a text string at
* the console.
*/
class ExampleProgram {
 public static void main(String[] args){
  System.out.println(&quot;I'm a Simple Program&quot;);
 }
}
</font></pre>
        <font face="Verdana">With one simple class, there is no reason
        to generate API documentation. API documentation makes sense
        when you have an application made up of a number of complex
        classes that need documentation. The tool generates <code>HTML</code>
        files (Web pages) that describe the class structures and contain
        the text enclosed by doc comments. The <a href="http://java.sun.com/products/jdk/javadoc/index.html" target="_blank">javadoc
        Home Page</a> has more information on the <code>javadoc</code>
        command and its output. <a name="api"></a></font>
        <h3><font face="Verdana">API Documentation</font></h3>
        <font face="Verdana">The Java platform installation includes API
        Documentation, which describes the APIs available for you to use
        in your programs. The files are stored in a <code>doc</code>
        directory beneath the directory where you installed the
        platform. For example, if the platform is installed in <code>/usr/local/java/jdk1.2</code>,
        the API Documentation is in <code>/usr/local/java/jdk1.2/doc/api</code>.
        <a name="more"></a></font>
        <h3><font face="Verdana">More Information</font></h3>
        <font face="Verdana">See <a href="http://java.sun.com/products/jdk/1.2/docs/tooldocs/tools.html" target="_blank">Java
        2 SDK Tools</a> for more information on setting the class path
        and using the <code>javac</code>, and <code>java</code>
        commands.</font>
        <p><font face="Verdana">See <a href="http://java.sun.com/docs/books/tutorial/getStarted/problems/index.html" target="_blank">Common
        Compiler and Interpreter Problems</a> lesson in <a href="http://java.sun.com/docs/books/tutorial/trailmap.html" target="_blank">The
        Java Tutorial</a> for troubleshooting help.</font>
        <p><font face="Verdana">The <a href="http://java.sun.com/products/jdk/javadoc/index.html" target="_blank">javadoc
        Home Page</a> has more information on the <code>javadoc</code>
        command and its output.</font>
        <p><font face="Verdana">You can also view the API Documentation
        for the Java 2 Platform on the <a href="http://java.sun.com/products/jdk/1.2/docs/api/index.html" target="_blank">java.sun.com</a>
        site.</font>
        <p><font face="Verdana">_______<br>
        <a name="TJVM"><sup>1</sup></a> As used on this web site, the
        terms &quot;Java virtual machine&quot; or &quot;JVM&quot; mean a
        virtual machine for the Java platform.</font>
        <hr>
        <!--BEGIN READER SURVEY-->
        <font size="2">
        <p><font face="verdana,arial"><b>Reprinted with permission from
        the <a href="http://developer.java.sun.com/developer/" target="_blank">Java
        Developer Connection(SM)</a><br>
        Copyright <a href="http://www.sun.com" target="_blank">Sun
        Microsystems Inc</a>.</b></font></p>
        </font>
        <p align="right"><font face="Verdana" size="-1">[<a href="#top">TOP</a>]</font></p>
       </td>
      </tr>
     </tbody>
    </table>
    <font face="Verdana, Arial, Helvetica, sans-serif"><!-- ================ -->
    <!-- End Main Content -->
    <!-- ================ -->
    </font></td>
  </tr>
 </tbody>
</table>
<!-- Copyright Insert -->

