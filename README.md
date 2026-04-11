   Topic : Basics of SAP and ABAP

1) ERP 
   Enterprise Resource Planning
   It's purpose is to manage any company functions.

2) SAP
   SAP - System Application and Products for real time data processing.
                             or
   SAP - System Application and Products in real time data processing.

3) History of SAP
   SAP introduced by SAP AG in 1972 at Walldorf.( Germany)
   SAP is a German based product.

4) Features of SAP
   a)It is an integration of all functions in to one common software.
   b)It is a Multi-lingual software.
   C)It is a user-based license aggrement.( requires user name and password)

5) SAP R/3 Architecture
   ( 3 - 3 tier architecture , R- Real) - SAP is a real time architecture.

   Layers - Presentation Layer( User Interaction Layer)



            Application Layer( Writing the programs and applications)

         Dispatcher:
         All requests that come in from presentation servers are directed first to dispatcher.
         The dispatcher writes them first to the dispatcher queue.
         The dispatcher pulls the requests from the queue on a first-in, first-out basis.


         Work Process:
         Each request from the dispatcher is then allocated to the first available work process. 
         A work process handles one request at a time.
         A work process needs to address two special memory areas - the user context and the program roll area. 


         User Context:
         The user context is a memory area that contains information about the user.
         When a user logs on, a user context is allocated for that logon.
         When a user log off, it is freed.


        Roll Area

         Roll area is a memory area that contains information about the program execution .
         When a program runs, a roll area is allocated for that program.
         The roll area is freed when the program ends.


         Database Layer( To store and retrive the data).

7) SAP Netweaver
   SAP NetWeaver(NW) is an integrated technology platform which can support various SAP applications.
   Examples -> SAP ERP(Enterprise Resource Planning)
               SAP CRM( Customer relationship Management)
               SAP SRM( Supply Relationship Management)
               SAP PI( Process Integration).

8) ABAP/4 -> 
   Advanced Business Application Programming language.
   It is a 4th generation language.
   ABAP lies on application Layer.

 

9) Modules of SAP->
   Functional Modules
   Technical Modules

   Functional Modules -> 
   SAP SD( Sales & Distribution) 
   SAP MM( Material Management)
   SAP PS( Project System)
   SAP FICO( Finance & Controlling)
   SAP HR( Human Resources) -> HCM( Human Capital Management)
   SAP WM( Warehouse Management)

   Techical Modules->
   SAP BASIS -> Administration and Monitoring of SAP systems.
   SAP ABAP -> Programming language for SAP.
   SAP BIBO( Business Intelligence , Business Objects) -> Reporting tool


10) SAP system Landscape

   Development - Dedicated for development.
   Quality -> Testing
   Production( Live system) - Used by the customer.

   Development->Quality->Production

   Transport Request -> It is a Mechanism to transport the objects from one system to another system.



SAP GUI
-------
G - Graphical U - User I - Interface
It allows end users to use various SAP applications by providing easy to use graphical interface.

3 Types of SAP GUI:
---------------------
SAP GUI for Windows - SAP GUI for windows is a windows operating system that offers a windows like user experience.
SAP GUI for JAVA - SAP GUI for JAVA environment is written in JAVA and is the platform-independent implementation of SAP GUI.  
SAP GUI for HTML - Consist of Internet Transaction Server (ITS) on the server side and a web browser on the client side.



11) SAP Logon Configuration:
------------------------------

   Description: You can put any description of the system.
   If we will not put any description, It is a combination of System Id and Application Server.
 
   Application Server: Enter IP address or Hostname of SAP application server.

   Instance number: Instance number of SAP system which is defined during SAP installation.  
                    It is of 2 characters long.It varies from 00 to 99.

   System ID(SID): System id is a unique identification code for every SAP system which is defined
                   during SAP Installation. 
                   It is of 3 characters long.
                   Example : S4H,A4H etc.


- In the windows server, you can see app SAP LOGON 770, click on SAP Logo
- click on new button, click on connection , click on next
- Description: AB4[SAPSERVER]  (This will come automatically which is concatenation of Systemid and application Server)
- Application Server : SAPServer
- Instance Number: 15
- System ID  : AB4
- SAProuter String:
- click on next, click on finish
- Now you can see ther server entry in the SAP GUI
- Now right click on the SAPServer  and click on properties to check
- Now to connect, double click SAPServer
- You will see as such
  Client  800
  User
  Password
  Logon language
- 



Features of SAP GUI 

- A single face GUI for accessing all SAP applications such as
    ERP(Enterprise resource planning),
     CRM(Customer Relationship Management),
      SAP SRM(Supply Relationship Management),
      PI(Process Integration) etc.
  
- Users are allowed to login with their preferred language, as the same GUI can be used in different languages

- It contains user parameters that are defined for more frequently keyed inputs. This enables the automatic population of text , based on specific user logins. This   in result, reduces the percentage of user inputs in real time.

- SAP GUI allows to configure GUI font size, colors, logos, custom layouts etc.

   - click on color, options and there you can select font and color sizes
  

- Elements of SAP GUI(Parts of SAP GUI) 

Menu Bar
The menu bar appears on the top of every SAP screen.
The menu bar changes from screen to screen.
System and help menus are always available on every screen.


Standard Toolbar(Function Keys)
The standard toolbar is located below the menu bar.
The standard toolbar buttons are also called as function keys.

Command Bar 
Command bar is used to enter the transaction codes.
Command bar can be opened and closed by using the icon on the right of the command bar.


Title Bar
In between the standard toolbar and the application toolbar lies the title bar.
It is used to display the name of the screen or application you are accessing.
Title bar is dynamic and changes from application to application.


Application Toolbar
The application toolbar is located directly below the title bar.
It contains buttons that duplicate functions available from the menu bar, but provides quicker access to some of the most commonly used functions for the current screen.
The buttons available in the application toolbar changes from application to application


Screen Area
The screen area of  SAP GUI is the area where the actual application is displayed.
It consists of layout elements like - buttons, input fields, radio buttons, checkboxes etc.


Status Bar
The status bar is located at the bottom of the SAP screen.
It displays important messages such as errors and completion of transactions.
It also displays the session information also such as system, client, user, program, transaction etc. 


SAP Easy Access - Adding Existing Item as Favorite 
----------------------------------------------------
Choose the existing item from the User Menu.
Click on Favorites - Add

SAP Easy Access - Adding New Item as Favorite 
----------------------------------------------------
Click on Favorites - Insert transaction

ABAP Workbench 




12) ABAP Workbench -> It is a collection of ABAP tools.
   SE38 -> Program/Report
   SE11-> ABAP Dictionary
   SE37 -> Function Module
   SE24-> Class

13) Transaction Code -> It is a shortcut to access ABAP workbench tools.

Examples : 

  /nxxxx - to call Transaction xxxx( override the existing session)

  /oxxxx - to Call Transaction xxxx in a new Session

  /NEX -> to close all the sessions

  /n -> to cancel a session

  /o- Display an Overview of sessions

14) User can open a maximum of 6 sessions.

15) F4 Help -> It tells us what are the various possible values for any Input field.
    F1 Help -> It gives us the technical information of any field/column.

          
                                 Topic : SAP Specific Objects and Customer Specific Objects.

1) Custom objects - starts with Z or Y.

2) SAP specific objects - other than Z or Y.

                                 Topic : Concept of Object Navigator, Package, Transport Request

SE80-> Object Navigator

Package -> It is a collection/container for the objects.( Table, Data element, Domains, Structures,Programs etc.)
In SAP, every object stored in to a package.

( Package for local objects : $TMP , local objects can never be transported)

SE21-> To create a package.

Transport request -> Medium to transport the objects.
SE09 -> To create a transport request.( Workbench request)



                      Topic : Main Tables and Transaction codes for Different Modules of SAP
                                  ( Concept of Header and Item Tables)

1) SAP Sales & Distribution(SD) ->
   Sales Order Details  
   Transaction codes - VA01( Sales Order Create)
                       VA02( Sales Order Change)
                       VA03( Sales Order Display)    


   Tables- VBAK( Sales Document Header)
           VBAP( Sales document Item)

   Billing Document Details
   Transaction codes -> VF01( Billing Document Create)
                        VF02( Billing Document Change)
                        VF03( Billing Document Display) 

 
   Tables -     VBRK(Billing Document Header) 
                VBRP( Billing Document Item) 

2) SAP Material Management(MM) -> 
   Material Master   
   Transaction codes - MM01( Material Create)
                       MM02( Material Change)
                       MM03( Material Display)   


   Tables - MARA( Material data)
            MAKT( Material Description)

3) SAP FI(Finance) -> 
   Accounting Document -> 
   Transaction codes - FB01( Accounting Document Create)
                       FB02( Accounting Document Change)
                       FB03( Accounting Document Display) 


  Tables- BKPF( Accounting document header) 
          BSEG( Accouting document item)
  
              
                                              
