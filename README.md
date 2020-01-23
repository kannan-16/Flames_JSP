To create Flames Application in java using JSP, you need to know what is FLAMES. If you are a 90’s kid, you definitely would not require any assistance on this. You are already a pro !!!

If you say you were a good kid back then in your school days, then let me explain you. FLAMES is an innovative game founded by a desperately single 90’s kid. This game would not employ you much, but your name and your crush’s name. 

Getting back to school days once again!!!
Take a sheet of paper, write your name and your crush’s name. Cancel off all the common characters you both have in your names. Now count the remaining uniques characters. Write the word FLAMES. To expand FLAMES, F stands for Friends, L stands for  Love, A - Affection, M - Marriage , E - Enemies, S - Siblings.  Cancel the character from the word FLAMES that comes as the unique character count. 

For example, if there are 10 unique characters in your names,
F L A M E S F L A M - come as the 10th character. Strike it off, You and your crush would not get married. Now your Flames would have F L A E S. Repeating the same, F L A E S F L A E S - Strike the S. And repeat the same till you get the final character. That is your ‘so called Flames’ relationship with your crush.

Now creating the application, 
Step 1: Open Eclipse, File —> New —> Dynamic Web Project. Give the project name as Flames. Select the target runtime Apache Tomcat v9.0 (it would have been selected by default). Click Next and Next once again. It comes to the Web Module phase. 
Make sure that Generate web.xml deployment descriptor is checked. Click Finish.

Now that your project is created you can see the source folder where you will have your servlets and java files. And you will have a web content folder where you will find META-INF and WEB-INF folders and inside WEB-INF folder you will have web.xml file. You can have your we deployment pages and JSP pages inside your WebContent. 

Step 2: Right click your WebContent —> New —> Others —> (search for JSP File). Name shall be check.jsp. You’d find the stater’s code. Change the title name inside the title tag. Create a form to get Your name and Your crush’s name. Use input tag to get your name and your crush’s name(let the name be “your” and  “crush”).
Inside the form tag, method shall be the method name where you direct it(say “post”), action shall be to the page that is redirected (say “FlamesCheck”). 

Step 3: Now create Servlet inside the src folder(that is where the Servlets and java folders go). The name of the folder is same as that of the file name given in the check.jsp under the form tag action property(we have kept it as FlamesCheck). Click next. It would have the URL mappings, have a clear note of it. Click Finish.

Step 4: Under the @WebServlet annotations, make sure the page is mentioned as “/FlamesCheck”, as we used it as our Servlet name. 

Step 5: Get the username and password using request.getParameter(“your”) and request.getParameter(“crush”) and store them individually in different variables (say your and crush. Preferred not to change the variable name). Now write the logic for FLAMES. Hope you know it!!!

Step 6: Create individual JSP files for Friends, Lovers, Affection, Marriage, Enemies and Siblings under the same WebContent folder.

Step 7: Design all the JSP files with suitable quotes and images.

Step 8: Get to the doPost method. We can redirect the page in two different methods. RequestDispatcher would be the best way, but we would use sendRedirect method, response.sendRedirect(“friends.jsp”), response.sendRedirect(“lovers.jsp”), etc.

Step 8: Inside the web.xml page eliminate all the welcome-file tags except anyone. Here remove the index.html and place check.jsp. This would load our first page.

Here I have been very skeptic in explaining the procedures of creating a JSP project. If you need any minute explanation, please contact your TM.

