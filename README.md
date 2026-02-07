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
            Database Layer( To store and retrive the data).

6) SAP Netweaver
   SAP NetWeaver(NW) is an integrated technology platform which can support various SAP applications.
   Examples -> SAP ERP(Enterprise Resource Planning)
               SAP CRM( Customer relationship Management)
               SAP SRM( Supply Relationship Management)
               SAP PI( Process Integration).

7) ABAP/4 -> 
   Advanced Business Application Programming language.
   It is a 4th generation language.
   ABAP lies on application Layer.

 

8) Modules of SAP->
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

11) SAP Logon Configuration:

   Description: You can put any description of the system.
   If we will not put any description, It is a combination of System Id and Application Server.
 
   Application Server: Enter IP address or Hostname of SAP application server.

   Instance number: Instance number of SAP system which is defined during SAP installation.  
                    It is of 2 characters long.It varies from 00 to 99.

   System ID(SID): System id is a unique identification code for every SAP system which is defined
                   during SAP Installation. 
                   It is of 3 characters long.
                   Example : S4H,A4H etc.

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
  
              
                                              
