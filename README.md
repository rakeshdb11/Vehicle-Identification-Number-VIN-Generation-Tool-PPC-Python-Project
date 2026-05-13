# Vehicle-Identification-Number-VIN-Generation-Tool-PPC-Python-Project

**Description** This project develops a Python-based VIN generation tool for automobile industry. A Vehicle Identification Number (VIN) is a globally recognized code that uniquely identifies each vehicle. For automobile industry, VINs are critical for manufacturing records, regulatory compliance, warranty tracking, and fleet management.
The tool ensures VINs are generated according to the given model and Variant wise structure.

**Terminology used in Project:-**
1) MODEL_NAME --> It Represents the Model Name that is Used for Product Selling in Market.
2) MODEL_CODE --> It Represents the system code of that particular model that is used for Company internal Purposes and system transactions.(Production planning/ tracking & Inventory Controlling).
3) CHECK DIGIT --> The check digit in a Vehicle Identification Number (VIN) is the character, used as a mathematical safeguard to verify that the VIN is valid and not mistyped or altered. It helps detect errors in transcription and ensures the authenticity of the VIN.
4)  START_SERIAL_NO --> It represents the starting serial number structure of that particular model or variant.
5)  JOB_CODE --> When manufacturers generate VINs, they often include internal codes that represent specific details about the vehicle. One of these is referred to as a Job Code.
   - A Job Code is an internal production or assembly code used by manufacturers to identify a particular build, order, or 
    job during the manufacturing process.

    Pupose:-
    - Links the VIN to a specific production job/order in the factory.
    - Helps track manufacturing batches and assembly line details.
    - Ensures traceability for quality control, warranty claims, and recalls
6) PREFIX --> In the context of a Vehicle Identification Number (VIN), the term “prefix” usually refers to the starting characters of the VIN, that will same for EVery VIN of that particular Model.
7) MONTH_CODE --> It represents the Month in which Vehicle VIN is Created, Sometimes this code will vary model to model.
   same month has different month_code for different models, you have to maintain month code of all models.
8) YEAR_CODE -->  It represents the Year in which Vehicle VIN is Created, Sometimes this code will vary model to model.
   same Year has different Year_code for different models, you have to maintain Year code of all models.

**Overview:-**

1) Two Excel Workbooks are attached with this Project.

   a) MODEL_INFORMATION --> This sheet consists the all model wise data related to VIN Structures. This workbook has 7 different sheets, every sheets are serving different 
      purposes. (Do not change name of any sheet.)
   
      **--> Sheet1 (CHESIS_NO)** :- Output of above project that is Vehicle Identification number will show in this sheet as per below Format.
   
   <img width="428" height="60" alt="image" src="https://github.com/user-attachments/assets/a03b2cf9-2811-4942-9300-77e3e8ecf1ee" />
     
      Here,
   
      Date --> It represents for which date you have released the sequence.
   
      Prod_Seq --> It represents the Production sequence number in that month.
   
      Job_No --> It represents internal job ID that is allocated to particular VIN for internal tracking.
   
      Model --> It represents the Model code.
   
      Serial_No. --> It represents the Vehicle Identification Number.

      **--> Sheet2(SEQ)** --> In this sheet you have to input the sequence of Model code with qty and date for VIN / JOB and Production sequence No. creation.
   
<img width="190" height="58" alt="image" src="https://github.com/user-attachments/assets/6f9a66ec-b2a1-43e0-806c-8c47b32ec706" />

      **--> Sheet3(MODEL)** -->  In this sheet you have to maintain the Structure of VIN against of each model code. this sheet works as a model master maintenaince for VIN Creation.

<img width="892" height="111" alt="image" src="https://github.com/user-attachments/assets/6b0e1c74-ec74-4708-b0b0-a7b0fb1ee702" />

Here, 
1) MODEL_NAME --> You have to input here, the sales name of that particular model or variant.
2) MODEL_CODE --> You have to enter the model code of that particular model that company are using for internal tracking or system transactions.
3) PREFIX --> This is the part of VIN Structure of that model, you have to enter those letter/ digits in this field that will  use in every single unit production of that model and will not change.
4) CHECK_DIGIT --> This is the check digit that maximum companies are using it to safequard the unqiueness of that particular VIN, and this digit will calculated by formula that you will maintained in code base and this unique for every VIN.
5) STRUCTURE_1 --> In Structure_1 various methodology is used to define structure and it will varry model to model structure. In some model it is Production Month_code of that model and in some it is Production Year Code and some leaves as blank or hyphen.
6) STRUCTURE_2 --> It is same as Structure 1, if there is month code in structure_1 then structure_2 is year code or vice-versa.
7) STRUCTURE_3 --> It is same as Structure 1 and 2,, all there structure are sharing three information month code, year code and one special digit/ character.
8) STRUCTURE_4 --> It represents the serial no. series of that model.
9) START_SERIAL_NO --> It gives the information, what will be the serial no. of first unit if that particular model.
10) SERIAL_NO_GROUP_NAME --> Some model has same serial number series but different VIN Structure for that we have to create the group methodology for all those model that are sharing the same serial number series. all model that are in same group will share same series.
11) LAST_SERIAL_NO --> It represent that last serial number against the GROUP_NAME that was in last VIN Creation cycle.
12) JOB_CODE --> As explained earlier job code is the internal tracking code to hold/release the lot and particular VIN in case of any abnormality. this has also some uniqueness that will change model to model. in this column you have to maintain that unique JOB code.
13) LAST_JOB_NO.--> It represents the last job no that was created in last VIN Creation cycle against all models.

**--> Sheet4 (MONTH_CODE)**
In this sheet you have to maintain the Group wise Month code, As per below Image.

<img width="737" height="106" alt="image" src="https://github.com/user-attachments/assets/497aaa1a-84cd-4460-8ca8-2ed3bdf6ec8f" />


**Sheet5 (YEAR_CODE)** -->
In this sheet you have to maintain the Group wise Year code, As per below Image.

<img width="304" height="90" alt="image" src="https://github.com/user-attachments/assets/05758740-4834-41dd-af57-8eb9d9e9c0d0" />

**Sheet5 & 6 (ISO Letter and digit)** --> This sheet is used to calculate the check digit, it is unique and decided by company.

   b) VIN_CREATION_HISTORY --> This sheet maintains the Past VIN Creation history with their time stamp. To ensure their is no duplicacy in VIN NO. , JOB NO. AND PRODUCTION SEQUENCE.

![Uploading image.png…]()

   
   




