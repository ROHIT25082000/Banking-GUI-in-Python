from tkinter import *
import tkinter.messagebox
def tip():
    root15=Tk()
    root15.title("SUGGESTIONS & TIPS")
    root15.geometry("500x500")
    state="IMPROVING IS THE KEY TO SUCCESS ,FILL THE ENTRY TO HELP US IMPROVE"
    msg= Message(root15,text=state)
    msg.config(fg="white",bg="lightgreen",font=("verdena",20,"italic"))
    msg.pack()
    entrytip=Entry(root15)
    entrytip.pack()
    def catch():
        f2=open("suggestion.txt","a")
        f2.write(entrytip.get()+"\n")
        labelres=Label(root15,text="---Thank You---",fg="purple",bg="white")
        labelres.pack()

    buttontip=Button(root15,text="_SUBMIT",fg="red",bg="yellow",command=catch)
    buttontip.pack()
    
   

    root15.mainloop()

def security():
    root13=Tk()
    root13.title("!!!Innovative security services.!!!")
    root13.geometry("600x400")

    label2=Label(root13,text="******WELCOME TO OUR SECURITY******",fg="purple",bg="white")
    label2.grid(row=0,sticky="n")

    label1=Label(root13,text="Enter your name",fg="purple",bg="white")
    label1.grid(row=1,sticky="w")

    entry1=Entry(root13)
    entry1.grid(row=1,column=2)

    label2=Label(root13,text="Enter D.O.B(-)",fg="purple",bg="white")
    label2.grid(row=2,sticky="w")

    entry2=Entry(root13)
    entry2.grid(row=2,column=2)

    label3=Label(root13,text="Enter your income",fg="purple",bg="white")
    label3.grid(row=3,sticky="w")

    entry3=Entry(root13)
    entry3.grid(row=3,column=2)
    
    label4=Label(root13,text="Enter your Aadhar",fg="purple",bg="white")
    label4.grid(row=4,sticky="w")

    entry4=Entry(root13)
    entry4.grid(row=4,column=2)

    label5=Label(root13,text="Enter your wife or father name",fg="purple",bg="white")
    label5.grid(row=5,sticky="w")

    entry5=Entry(root13)
    entry5.grid(row=5,column=2)

    
    def protect():
       
        codes = { 'A':'.-', 'B':'-...', 
                    'C':'-.-.', 'D':'-..', 'E':'.', 
                    'F':'..-.', 'G':'--.', 'H':'....', 
                    'I':'..', 'J':'.---', 'K':'-.-', 
                    'L':'.-..', 'M':'--', 'N':'-.', 
                    'O':'---', 'P':'.--.', 'Q':'--.-', 
                    'R':'.-.', 'S':'...', 'T':'-', 
                    'U':'..-', 'V':'...-', 'W':'.--', 
                    'X':'-..-', 'Y':'-.--', 'Z':'--..', 
                    '1':'.----', '2':'..---', '3':'...--', 
                    '4':'....-', '5':'.....', '6':'-....', 
                    '7':'--...', '8':'---..', '9':'----.', 
                    '0':'-----', ', ':'--..--', '.':'.-.-.-', 
                    '?':'..--..', '/':'-..-.', '-':'-....-', 
                    '(':'-.--.', ')':'-.--.-'}
        value1=entry1.get()
        value2=entry2.get()
        value3=entry3.get()
        value4=entry4.get()
        value5=entry5.get()
        

        
        if len(value1) and len(value2) and len(value3) and len(value4) and len(value5)>0:

            root14 = Tk()
            root14.geometry("1200x500")
            root14.title("MORSE :The modern security expert....")

            def encrypt(message): 
                x = '' 
                for letter in message: 
                    if letter != ' ': 
  
            
                       x += codes[letter] + ' '
                    else: 
           
                        x += ' '
  
                return x
        
            

            label1=Label(root14,text="NAME in MORSE",fg="orange",bg="white")
            label1.grid(row=0,sticky="w")

            label2=Label(root14)
            label2["text"]= encrypt(value1.upper())
            label2.grid(row=0,column=1)

            label3=Label(root14,text="D.O.B in MORSE",fg="orange",bg="white")
            label3.grid(row=1,sticky="w")

            label4=Label(root14)
            label4["text"]= encrypt(value2.upper())
            label4.grid(row=1,column=1)

            label5=Label(root14,text="INCOME in MORSE",fg="orange",bg="white")
            label5.grid(row=2,sticky="w")

            label6=Label(root14)
            label6["text"]= encrypt(value3.upper())
            label6.grid(row=2,column=1)

            label7=Label(root14,text="AADHAR in MORSE",fg="orange",bg="white")
            label7.grid(row=3,sticky="w")

            label8=Label(root14)
            label8["text"]= encrypt(value4.upper())
            label8.grid(row=3,column=1)

            label9=Label(root14,text="WIFE OR FATHER NAME in MORSE",fg="orange",bg="white")
            label9.grid(row=4,sticky="w")

            label10=Label(root14)
            label10["text"]= encrypt(value5.upper())
            label10.grid(row=4,column=1)

            labelwarn=Label(root14,text="DEAR USERS\n This morse code is the most valuable asset of PESU Bank\n 100% security of info is Guaranteed",fg="purple",bg="yellow")
            labelwarn.grid(row=6,sticky="w")
            status=Label(root14,text="Securing your details >>>.... -by BHAVANI SHANKAR,PES1201801864------",relief =SUNKEN,anchor=W,bd=1)
            status.grid(row=10,column=2)
            root14.mainloop()            
        else:
            labelq=Label(root13,text="*__* ENTER DETAILS CAREFULLY *__*",fg="red",bg="yellow")
            labelq.grid(row=8,column=17)
    button1=Button(root13,text="_Submit",fg="blue",bg="orange",command=protect)
    button1.grid(row=7,column=15)
    
    root13.mainloop()
#################
def home_loan():
    root7=Tk()
    root7.geometry("1200x150")
    root7.title("Home_loans")

    label_homeloan1=Label(root7,text="Enter your full name",fg="orange",bg="white")
    label_homeloan1.grid(row=0,sticky="w")

    label_homeloan2=Label(root7,text="Enter the builders Name" ,fg="orange",bg="white")
    label_homeloan2.grid(row=1,sticky="w")

    label_homeloan3=Label(root7,text="Enter the Name of the witness " ,fg="orange",bg="white")
    label_homeloan3.grid(row=2,sticky="w")

    label_homeloan4=Label(root7,text="Enter the name of your wife or father" ,fg="orange",bg="white")
    label_homeloan4.grid(row=3,sticky="w")

    label_homeloan5=Label(root7,text="house area in 'in square_feet'",fg="orange",bg="white")
    label_homeloan5.grid(row=4,sticky="w")

    entry1=Entry(root7)
    entry1.grid(row=0, column=1)

    
    entry2=Entry(root7)
    entry2.grid(row=1, column=1)
    
    
    entry3=Entry(root7)
    entry3.grid(row=2, column=1)
    

    entry4=Entry(root7)
    entry4.grid(row=3, column=1)
    
    entry5=Entry(root7)
    entry5.grid(row=4, column=1)
    def sanction():
        value = entry1.get()              
        value1= entry2.get()
        value2= entry3.get()
        value3= entry4.get()
        value4= entry5.get() 
        air="***CONGRATULATIONS!! LOAN SANCTIONED ***\nCOLLECT THE SANCTION LETTER FROM THE OFFICE\n THE INTEREST RATE IS 6%pa "
        labelsanction=Label(root7)
    

        if len(value)and len(value1) and len(value2) and len(value3) and len(value4) >0:
            labelsanction["text"]= air 
            labelsanction.grid(row=5,column=5)
    check_enter=Checkbutton(root7, text="I agree to all terms and conditions of the loan")
    check_enter.grid(row=5,column=3)
    button_enter=Button(root7,text="SUBMIT",fg="green", bg="cyan",command=sanction)
    button_enter.grid(row=6,column=3)
    root7.mainloop()
#####################
def car_loan():
    root9=Tk()
    root9.geometry("1200x150")
    root9.title("Car_loans")

    label_homeloan1=Label(root9,text="Enter your full name",fg="orange",bg="white")
    label_homeloan1.grid(row=0,sticky="w")

    label_homeloan2=Label(root9,text="Enter name of the car " ,fg="orange",bg="white")
    label_homeloan2.grid(row=1,sticky="w")

    label_homeloan3=Label(root9,text="Enter the Name of the witness " ,fg="orange",bg="white")
    label_homeloan3.grid(row=2,sticky="w")

    label_homeloan4=Label(root9,text="Enter the name of your wife or father" ,fg="orange",bg="white")
    label_homeloan4.grid(row=3,sticky="w")

    label_homeloan5=Label(root9,text="Enter the model,colour",fg="orange",bg="white")
    label_homeloan5.grid(row=4,sticky="w")

    entry1=Entry(root9)
    entry1.grid(row=0, column=1)

    
    entry2=Entry(root9)
    entry2.grid(row=1, column=1)
    
    
    entry3=Entry(root9)
    entry3.grid(row=2, column=1)
    

    entry4=Entry(root9)
    entry4.grid(row=3, column=1)
    
    entry5=Entry(root9)
    entry5.grid(row=4, column=1)
    def sanctioncar():
        value = entry1.get()              
        value1= entry2.get()
        value2= entry3.get()
        value3= entry4.get()
        value4= entry5.get() 
        air="***CONGRATULATIONS!! LOAN SANCTIONED ***\nCOLLECT THE SANCTION LETTER FROM THE OFFICE\n THE INTEREST RATE IS 8%pa "
        labelsanctioncar=Label(root9)
    

        if len(value)and len(value1) and len(value2) and len(value3) and len(value4) >0:
            labelsanctioncar["text"]= air 
            labelsanctioncar.grid(row=5,column=5)
    check_enter=Checkbutton(root9, text="I agree to all terms and conditions of the loan")
    check_enter.grid(row=5,column=3)
    button_enter=Button(root9,text="SUBMIT",fg="green", bg="cyan",command=sanctioncar)
    button_enter.grid(row=6,column=3)
    root9.mainloop()
########################
def student_loan():
    root10=Tk()
    root10.geometry("1200x150")
    root10.title("Student_loan")
    label_homeloan1=Label(root10,text="Enter your full name",fg="orange",bg="white")
    label_homeloan1.grid(row=0,sticky="w")

    label_homeloan2=Label(root10,text="Enter the name of institution" ,fg="orange",bg="white")
    label_homeloan2.grid(row=1,sticky="w")

    label_homeloan3=Label(root10,text="Enter the Name of the course,fees " ,fg="orange",bg="white")
    label_homeloan3.grid(row=2,sticky="w")

    label_homeloan4=Label(root10,text="Enter the name of your wife or father" ,fg="orange",bg="white")
    label_homeloan4.grid(row=3,sticky="w")

    label_homeloan5=Label(root10,text="Enter the period of the course 20xx-20yy",fg="orange",bg="white")
    label_homeloan5.grid(row=4,sticky="w")

    entry1=Entry(root10)
    entry1.grid(row=0, column=1)

    
    entry2=Entry(root10)
    entry2.grid(row=1, column=1)
    
    
    entry3=Entry(root10)
    entry3.grid(row=2, column=1)
    

    entry4=Entry(root10)
    entry4.grid(row=3, column=1)
    
    entry5=Entry(root10)
    entry5.grid(row=4, column=1)
    def sanction():
        value = entry1.get()              
        value1= entry2.get()
        value2= entry3.get()
        value3= entry4.get()
        value4= entry5.get() 
        air="***CONGRATULATIONS!! LOAN SANCTIONED ***\nCOLLECT THE SANCTION LETTER FROM THE OFFICE\n THE INTEREST RATE IS 4%pa "
        labelsanction=Label(root10)
    

        if len(value)and len(value1) and len(value2) and len(value3) and len(value4) >0:
            labelsanction["text"]= air 
            labelsanction.grid(row=5,column=5)
    check_enter=Checkbutton(root10, text="I agree to all terms and conditions of the loan")
    check_enter.grid(row=5,column=3)
    button_enter=Button(root10,text="SUBMIT",fg="green", bg="cyan",command=sanction)
    button_enter.grid(row=6,column=3)
    root10.mainloop()
######################
def food_coupons():
    root11=Tk()
    root11.geometry("1200x350")
    root11.title("PES FOOD COUPONS: HUNGER ENDS HERE......Discover great coupons to eat around !!")
    label_homeloan6=Label(root11,text="COUPONS AVAILABLE\n      BREAKFAST COUPON @ Rs 5per coupon\n     LUNCH COUPON @ Rs 10 per coupon\n      DINNER COUPONS @ Rs 15 per coupon",fg="green" ,bg="white")
    label_homeloan6.grid(row=0,sticky="w")


    label_homeloan1=Label(root11,text="Enter your full name",fg="orange",bg="white")
    label_homeloan1.grid(row=1,sticky="w")

    label_homeloan2=Label(root11,text="Enter your room No or class" ,fg="orange",bg="white")
    label_homeloan2.grid(row=2,sticky="w")

    label_homeloan3=Label(root11,text="Enter the name of mess(NORTH INDIAN|SOUTH INDIAN)" ,fg="orange",bg="white")
    label_homeloan3.grid(row=3,sticky="w")

    label_homeloan4=Label(root11,text="Enter the your SRN" ,fg="orange",bg="white")
    label_homeloan4.grid(row=4,sticky="w")

    label_homeloan5=Label(root11,text="Enter the no of coupons needed",fg="orange",bg="white")
    label_homeloan5.grid(row=5,sticky="w")

    label_homeloan7=Label(root11,text="Select the type of coupon ")
    label_homeloan7.grid(row=6,sticky="w")

   
    entry1=Entry(root11)
    entry1.grid(row=1, column=1)

    
    entry2=Entry(root11)
    entry2.grid(row=2, column=1)
    
    
    entry3=Entry(root11)
    entry3.grid(row=3, column=1)
    

    entry4=Entry(root11)
    entry4.grid(row=4, column=1)
    
    entry5=Entry(root11)
    entry5.grid(row=5, column=1)
    def b():
        value=int(entry5.get())
        labelhome_loan8=Label(root11)
        labelhome_loan8["text"]="Your total breakfast counpons costs"+" "+"Rs"+str(float(value*5))
        labelhome_loan8.grid(row=10,column=5)
    def l():
        value=int(entry5.get())
        labelhome_loan8=Label(root11)
        labelhome_loan8["text"]="Your total lunch coupons costs"+" "+"Rs"+str(float(value*10))
        labelhome_loan8.grid(row=10,column=5)
    def d():
        value=int(entry5.get())
        labelhome_loan8=Label(root11)
        labelhome_loan8["text"]="Your total dinner coupons costs"+" "+"Rs"+str(float(value*15))
        labelhome_loan8.grid(row=10,column=5)

    



       
    buttoncoupon=Button(root11,text="BREAKFAST COUPON",fg="blue",bg="yellow",command=b)
    buttoncoupon.grid(row=6,column=10)

    buttoncoupon1=Button(root11,text="LUNCH COUPON",fg="blue",bg="yellow",command=l)
    buttoncoupon1.grid(row=6,column=20)
    
    buttoncoupon2=Button(root11,text="DINNER COUPON",fg="blue",bg="yellow",command=d)
    buttoncoupon2.grid(row=6,column=30)



    def sanction():
        value = entry1.get()              
        value1= entry2.get()
        value2= entry3.get()
        value3= entry4.get()
        value4= entry5.get() 
        air="***CONGRATULATIONS!! FOOD COUPONS PURCHASED***\n FOOD COUPONS WILL DELIVERED TO YOU WITHIN 30min\n THE COUPONS CHARGES\INCLUDED IN THE FEES "
        
        labelsanction=Label(root11)
    

        if len(value)and len(value1) and len(value2) and len(value3) and len(value4) >0:
            labelsanction["text"]= air 
            labelsanction.grid(row=7,column=5)
    check_enter=Checkbutton(root11, text="I agree ")
    check_enter.grid(row=8,column=3)
    button_enter=Button(root11,text="Proceed to pay__",fg="green", bg="cyan",command=sanction)
    button_enter.grid(row=9,column=3)
    root11.mainloop()
########################
def travel_loans():
    root12=Tk()
    root12.geometry("1200x650")
    root12.title("PESU YATRA ....Making travel Simple!!!!....")
    label_homeloan1=Label(root12,text="Enter your full name",fg="orange",bg="white")
    label_homeloan1.grid(row=0,sticky="w")

    label_homeloan2=Label(root12,text="From " ,fg="orange",bg="white")
    label_homeloan2.grid(row=1,sticky="w")

    label_homeloan3=Label(root12,text="To " ,fg="orange",bg="white")
    label_homeloan3.grid(row=2,sticky="w")

    label_homeloan4=Label(root12,text="Start  date" ,fg="orange",bg="white")
    label_homeloan4.grid(row=3,sticky="w")

    label_homeloan5=Label(root12,text="Return date",fg="orange",bg="white")
    label_homeloan5.grid(row=4,sticky="w")

    label_homeloan6=Label(root12,text="Enter the no of passenger travelling",fg="orange",bg="white")
    label_homeloan6.grid(row=5,sticky="w")

    label_homeloan7=Label(root12,text="Enter the no of passenger travelling back ",fg="orange",bg="white")
    label_homeloan7.grid(row=6,sticky="w")
    
    label_homeloan8=Label(root12,text="Select the mode of travel",fg="orange",bg="white")
    label_homeloan8.grid(row=7,sticky="w")

   
        
    def t():
        value1 = entry1.get()              
        value2= entry2.get()
        value3= entry3.get()
        value4= entry4.get()
        value5= entry5.get() 
        value6= int(entry6.get())
        value7= int(entry7.get())
        def pt():
            n=[]
            l=["Rajdhani","Shatabadi","Durronto"]
            import random
            train=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            trainno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your Train is"+" "+train+"\n"+"Your train No:"+" "+str(trainno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your Train is"+" "+train+"\n"+"Your train No:"+" "+str(trainno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*2300))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*2300))
                totallabel2.grid(row=24,column=17)
        def ds():
            n=[]
            l=["intercity Superfast","Mahanagari Superfast","Deccan queen Superfast "]
            import random
            train=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            trainno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your Train is"+" "+train+"\n"+"Your train No:"+" "+str(trainno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your Train is"+" "+train+"\n"+"Your train No:"+" "+str(trainno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*1300))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*1300))
                totallabel2.grid(row=24,column=17)

        def gr():
            n=[]
            l=["Bagvati garib rath","Sampark garib rath ","Musafir garib rath"]
            import random
            train=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            trainno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your Train is"+" "+train+"\n"+"Your train No:"+" "+str(trainno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your Train is"+" "+train+"\n"+"Your train No:"+" "+str(trainno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*1000))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*1000))
                totallabel2.grid(row=24,column=17)       

        buttontrains1=Button(root12 ,text="Premium trains",fg="blue",bg="orange",command=pt)
        buttontrains1.grid(row=8,column=10)

        buttontrains2=Button(root12 ,text="Daily Superfast",fg="blue",bg="orange",command=ds)
        buttontrains2.grid(row=10,column=10)

        buttontrains3=Button(root12 ,text="Garib Rath",fg="blue",bg="orange",command=gr)
        buttontrains3.grid(row=12,column=10)


    def f():
        value1 = entry1.get()              
        value2= entry2.get()
        value3= entry3.get()
        value4= entry4.get()
        value5= entry5.get() 
        value6= int(entry6.get())
        value7= int(entry7.get())
        def business():
            n=[]
            l=["Lufthansa","Air India","Emirates","Qatar Airways","Kingfisher"]
            import random
            flight=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            flightno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your flight is"+" "+flight+"\n"+"Your flight No:"+" "+str(flightno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your flight is"+" "+flight+"\n"+"Your flight No:"+" "+str(flightno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*7000))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*7000))
                totallabel2.grid(row=24,column=17)
        def premiumeconomy():
            n=[]
            l=["Air Asia","Air India","Air India Express","GoAir","Indigo","Vistara","Jet Airways"]
            import random
            flight=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            flightno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your flight is"+" "+flight+"\n"+"Your flight No:"+" "+str(flightno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your flight is"+" "+flight+"\n"+"Your flight No:"+" "+str(flightno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*5300))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*5300))
                totallabel2.grid(row=24,column=17)

        def economy():
            n=[]
            l=["Jetlite","SpiceJet","AirCoasta","Air CarnivalJet","Airpegasus"]
            import random
            flight=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            flightno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your flight is"+" "+flight+"\n"+"Your flight No:"+" "+str(flightno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your flight is"+" "+flight+"\n"+"Your flight No:"+" "+str(flightno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*4000))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*4000))
                totallabel2.grid(row=24,column=17)       

        buttonflight1=Button(root12 ,text="Business",fg="blue",bg="orange",command=business)
        buttonflight1.grid(row=8,column=20)

        buttonflight2=Button(root12 ,text="Premium Economy",fg="blue",bg="orange",command=premiumeconomy)
        buttonflight2.grid(row=10,column=20)

        buttonflight3=Button(root12 ,text="Economy",fg="blue",bg="orange",command=economy)
        buttonflight3.grid(row=12,column=20)


    def b():
        value1 = entry1.get()              
        value2= entry2.get()
        value3= entry3.get()
        value4= entry4.get()
        value5= entry5.get() 
        value6= int(entry6.get())
        value7= int(entry7.get())
        def sleeperAC():
            n=[]
            l=["SRS Travels","VRL Travels","VOLVO","HEBRON","K.S.R.T.C"]
            rajya=["KA-","MH-","TN-","UP-","RJ-","GJ-","KL-","WB-","MP-","AP-","DL-"]
            import random
            busstate=random.choice(rajya)
            bus=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            busno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your bus is"+" "+bus+"\n"+"Your bus No:"+busstate+" "+str(busno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your bus is"+" "+bus+"\n"+"Your bus No:"+busstate+" "+str(busno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*1500))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*1500))
                totallabel2.grid(row=24,column=17)
        def semisleeperAC():
            n=[]
            l=["SRS Travels","VRL Travels","VOLVO","HEBRON","K.S.R.T.C"]
            rajya=["KA-","MH-","TN-","UP-","RJ-","GJ-","KL-","WB-","MP-","AP-","DL-"] 
            import random
            busstate=random.choice(rajya)
            bus=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            busno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your bus is"+" "+bus+"\n"+"Your bus No:"+busstate+" "+str(busno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your bus is"+" "+bus+"\n"+"Your bus No:"+busstate+" "+str(busno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*900))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*900))
                totallabel2.grid(row=24,column=17)

        def sleeperNonAC():
            n=[]
            l=["SRS Travels","VRL Travels","VOLVO","HEBRON","K.S.R.T.C"]
            rajya=["KA-","MH-","TN-","UP-","RJ-","GJ-","KL-","WB-","MP-","AP-","DL-"]
            import random
            busstate=random.choice(rajya)
            bus=random.choice(l)
            for i in range(1000,10000):
                n.append(i)
            busno=random.choice(n)
            labelticket=Label(root12)
            labelticket1=Label(root12)
            totallabel1=Label(root12)
            totallabel2=Label(root12)
            if len(value1)and len(value2) and len(value3) and len(value4) and len(value5) and len(str(value6)) >0:
                labelticket["text"]="first trip"+"\n"+"Your bus is"+" "+bus+"\n"+"Your bus No:"+busstate+" "+str(busno)+"\n"+"date"+value4+"\n"+"time 16:00"+"no of passengers"+str(value6)
                labelticket.grid(row=14,column=15)
                labelticket1["text"]="second trip"+"\n"+"Your bus is"+" "+bus+"\n"+"Your bus No:"+busstate+" "+str(busno)+"\n"+"date"+value5+"\n"+"time 10:00"+"no of passengers"+str(value7)
                labelticket1.grid(row=16,column=15)
                totallabel1["text"]="first_trip cost"+"=>>"+"Rs"+str(float((value6)*600))
                totallabel1.grid(row=20,column=17)
                totallabel2["text"]="second_trip cost"+"=>>"+"Rs"+str(float((value7)*600))
                totallabel2.grid(row=24,column=17)       

        buttonbus1=Button(root12 ,text="sleeperAC",fg="blue",bg="orange",command=sleeperAC)
        buttonbus1.grid(row=8,column=30)

        buttonbus2=Button(root12 ,text="semisleeperAC",fg="blue",bg="orange",command=semisleeperAC)
        buttonbus2.grid(row=10,column=30)

        buttonbus3=Button(root12 ,text="sleeperNonAC",fg="blue",bg="orange",command=sleeperNonAC)
        buttonbus3.grid(row=12,column=30)



    button1=Button(root12,text="Train_",fg="blue",bg="yellow",command=t)
    button1.grid(row=7,column=10)

    button2=Button(root12,text="Flight_",fg="blue",bg="yellow",command=f)
    button2.grid(row=7,column=20)

    button3=Button(root12,text="Bus_",fg="blue",bg="yellow",command=b)
    button3.grid(row=7,column=30)
    
    entry1=Entry(root12)
    entry1.grid(row=0, column=1)

    
    entry2=Entry(root12)
    entry2.grid(row=1, column=1)
    
    
    entry3=Entry(root12)
    entry3.grid(row=2, column=1)
    

    entry4=Entry(root12)
    entry4.grid(row=3, column=1)
    
    entry5=Entry(root12)
    entry5.grid(row=4, column=1)

    entry6=Entry(root12)
    entry6.grid(row=5,column=1)

    
    entry7=Entry(root12)
    entry7.grid(row=6,column=1)

    def sanctioncar():
        value1 = entry1.get()              
        value2= entry2.get()
        value3= entry3.get()
        value4= entry4.get()
        value5= entry5.get() 
        value6= entry6.get()
        
        air="***CONGRATULATIONS!! TICKETS BOOKED ***\nTICKETS WILL BE GIVEN TO YOU WIHTIN 3 HOURS\n THE TICKET COST WILL BE INCLUDED IN THE FEES"
        labelsanctioncar=Label(root12)
    

        if len(value1)and len(value2) and len(value3) and len(value4) and len(value5)and len(str(value6)) >0:
            labelsanctioncar["text"]= air 
            labelsanctioncar.grid(row=5,column=5)
    check_enter=Checkbutton(root12, text="I hereby confirm my trip ")
    check_enter.grid(row=22,column=7)
    button_enter=Button(root12,text="Proceed to pay__",fg="green", bg="cyan",command=sanctioncar)
    button_enter.grid(row=24,column=7)
    root12.mainloop()
    
#############################
def enroll():
    root4=Tk()
    root4.geometry("400x200")
    root4.title("*_*OUR SERVICES*_*")

    button1=Button(root4 ,text="HOME LOANS",command=home_loan)
    button2=Button(root4 ,text="CAR LOANS " ,command=car_loan)
    button3=Button(root4 ,text="STUDENT LOANS",command=student_loan)
    button4=Button(root4 ,text="FOOD COUPONS ",command=food_coupons)
    button5=Button(root4 ,text="TRAVEL LOANS ",command=travel_loans)
    button1.pack()
    button2.pack()
    button3.pack()
    button4.pack()
    button5.pack()
    root4.mainloop()

def service():
    root3=Tk()
    root3.title("OUR SERVICES")
    root3.geometry("500x500")
    topframe=Frame(root3)
    topframe.pack()
    label=Label(topframe,text="OUR OTHER FEATURES:-\n HOME LOANS\nCAR LOANS\nSTUDENT LOANS\n FOOD COUPONS \n TRAVEL LOANS",fg="black")
    label.pack(side=LEFT)
    button=Button(root3, text ="Enroll Now",fg="blue",bg="white",command=enroll)
    button.pack(side=BOTTOM)
    root3.mainloop()
###################
def enter():
    root2=Tk()
    root2.title("SIGN UP_PAGE")
    root2.geometry("1200x150")

    label_enter1=Label(root2,text="Enter your first name",fg="violet",bg="white")
    label_enter1.grid(row=0,sticky='w')

    label_enter2=Label(root2,text="Enter your last name",fg="violet",bg="white")
    label_enter2.grid(row =1,sticky="w")

    label_enter3=Label(root2 ,text="Enter your age",fg="violet",bg="white")
    label_enter3.grid(row=2,sticky="w")

    label_enter4=Label(root2,text="Enter your gender ",fg="violet",bg="white")
    label_enter4.grid(row=3,sticky="w")


    def save():
        root5=Tk()
        root5.title("YOUR PERSONAL DETAILS")
        root5.geometry("1200x150")
        name_save = entry1.get()
        name1_save = entry2.get()
        age_save = entry3.get()
        gender_save = entry4.get()
        label_save1=Label(root5)
        label_save2=Label(root5)
        label_save3=Label(root5)
        label_save4=Label(root5)
    
        if len(name_save)and len(name1_save) and len(age_save) and len(gender_save) >0:
            label_enter5=Label(root2,text="----LOGIN SUCCESSFULL----")
            label_enter5.grid(row = 6, column=1)
            label_save1["text"]= name_save
            label_save2["text"]= name1_save
            label_save3["text"]= age_save
            label_save4["text"]= gender_save
            label_save1.grid(row=0,sticky="w")
            label_save2.grid(row=1,sticky="w")
            label_save3.grid(row=2,sticky="w")
            label_save4.grid(row=3,sticky="w")
            import random
            #for password
            l=[]
            for i in range(1000,10000):
                l.append(str(i))
            a=random.choice(l)
            f= open("pesudir.txt","a")
            f.write(name_save+"\n")
            f.write(name1_save+"\n")
            f.write(age_save+"\n")
            f.write(gender_save+"\n")
            f.write(str(a)+"\n")

            label_save5=Label(root5,text="YOUR PIN IS "+"===>  "+a,fg="green",bg="white")
            label_save5.grid(row=4,sticky="w")
        
        

    entry1=Entry(root2)
    entry1.grid(row=0 ,column=1)
    entry2=Entry(root2)
    entry2.grid(row=1 ,column=1)
    entry3=(Entry(root2))
    entry3.grid(row=2 ,column=1)
    entry4=Entry(root2)
    entry4.grid(row=3, column=1)
    check_enter=Checkbutton(root2, text="I agree to all terms and conditions of the bank")
    check_enter.grid(row=5,column=3)
    button_enter=Button(root2,text="SUBMIT",fg="green", bg="cyan",command=save)
    button_enter.grid(row=6,column=3)
    root2.mainloop()
########################    

#######################
def crow():
    root8=Tk()
    root8.geometry("700x200")
    root8.title("WITHDRAWAL")
    
    label1=Label(root8,text="----PLEASE INSERT THE CARD----",fg="orange",bg="white")
    label1.grid(row=1,column=5)
    label3=Label(root8,text="Available Denominations in 100x,200x,500x,2000x",fg="orange",bg="white")
    label3.grid(row=2,sticky="w")
    label2=Label(root8,text='Enter the amount',fg="orange",bg="white")
    label2.grid(row=3,sticky='w')
    enter1=Entry(root8)
    enter1.grid(row=3,column=6)
    label6=Label(root8,text="Enter the pin",fg="orange",bg="white")
    label6.grid(row=4,sticky='w')
    enter2=Entry(root8)
    enter2.grid(row=4,column=6)
    def money():
        value=enter1.get()
        pin=enter2.get()
        label4=Label(root8)
        label5=Label(root8)
        f=open("pesudir.txt","r")
        k=f.readlines()
        
        if len(value)>0 and pin+"\n" in k:
            label4["text"]= "transaction of "+"Rs"+"   "+value+"   "+"is getting processed"
            label4.grid(row=7,column=0)
            label7=Label(root8,text=k[k.index(pin+"\n")-4]+" "+k[k.index(pin+"\n")-3],fg="blue",bg="white")
            label7.grid(row=8,column=0)
        else:
            label5["text"]="Enter proper amount and pin carefully  "
            label5.grid(row=10,column=2)
    def rep():
        value=enter1.get()
        label5=Label(root8)
        label5["text"]="amount withdrawn"+""+"Rs"+value
        label5.grid(row=6,column=5)
    button2=Button(root8,text="RECEIPT",fg="orange",bg='white',command=rep)

    button2.grid(row=5,column=7)
    button1=Button(root8,text="Next_",fg="blue",bg="white",command=money)
    button1.grid(row=5,column=5)
    root8.mainloop()
###########################    
def moo():
    def result():
        value = (entry1.get())
        if (value) =="":
            label_moo_error=Label(root1,text="!!! PLEASE ENTER PROPER AMOUNT !!!",fg="red")
            label_moo_error.grid(row=3,column=2)
                                  
        string_to_display = "Rs"+" "+str(10000+float(value))
        label_moo=Label(root1)
        label_moo1=Label(root1)
        label_moo2=Label(root1)
        f=open("pesudir.txt","r")
        k=f.readlines()
        
        
        
        if len(value)>0 and entry2.get()+"\n" in k :
            label7=Label(root1,text=k[k.index(entry2.get()+"\n")-4]+" "+k[k.index(entry2.get()+"\n")-3],fg="blue",bg="white")
            label7.grid(row=10,column=0)
            label_moo["text"]= string_to_display
            label_moo.grid(row=2,column=2)
            label_moo1["text"]="*_* THANK YOU *_*"
            label_moo1.grid(row=3,column=2)
            label_moo2["text"]=">>>> YOUR NEW BALANCE <<<<"+"Rs"+" "+str(10000+float(value))
            label_moo2.grid(row=4,column=3)
        else :
            labelw=Label(root1,text="incorrect pin !TRY AGAIN",fg="red")
            labelw.grid(row=10,column=0)

    root1=Tk()
    root1.title("ADD MONEY")
    root1.geometry("600x600")
    labelmoo1=Label(root1,text="ENTER THE AMOUNT TO BE DEPOSITED",fg="cyan",bg="grey")
    labelmoo1.grid(row=0,sticky ="w")
    entry1=Entry(root1)
    entry1.grid(row=0,column=1)
    labelpin=Label(root1,text="Enter the pin",fg="orange",bg="white")
    labelpin.grid(row=1,sticky="w")
    entry2=Entry(root1)
    entry2.grid(row=1,column=1)

    button7=Button(root1,text="<<-DEPOSIT->>",command=result)
    button7.grid(row=0,column=3)
    button12=Button(root1)
    button12.grid(row=0,column=6)
    root1.mainloop()

root=Tk()
root.geometry("1100x900")
root.title("PESU BANK")
state="PESU"
msg= Message(root,text=state)
msg.config(fg="white",bg="lightgreen",font=("verdena",20,"italic"))
msg.pack()
state1="BANK"
msg1= Message(root,text=state1)
msg1.config(fg="white",bg="lightgreen",font=("verdena",20,"italic"))
msg1.pack()
label3=Label(root,text="Bank for life!! Zindagi ke saath bhi aur Zindagi ke baad bhi",fg="green",bg="yellow")
label3.pack()
label2=Label(root,text="PES UNIVERSITY",fg="orange")
label2.pack()
label9=Label(root,text="PLACE WHERE INDIA BANKS !!!!",fg="black",bg="orange")
label9.pack()
label5=Label(root,text="COME ONN!!! INDIA LET'S! BANK ",fg="red")
label5.pack()
label6=Label(root,text="OUR COSTUMERS ,OUR GOD ",fg="green")
label6.pack()
label7=Label(root,text="BELOW IS OUR USER GUI FOR VIRTUAL ATM",fg="violet",bg="yellow")
label7.pack()
label10=Label(root,text="-by ROHIT VISHWAKARMA PES1201800152",fg="brown",bg="white")
label10.pack(side="right")
button1=Button(root,text="start or LOGIN",command=enter)
button1.pack(side=LEFT)
button2=Button(root,text="-SUGGESTIONS & TIPS-",command=tip)
button2.pack(side=RIGHT)
button3=Button(root,text="-REFRESH-")
button3.pack(side=RIGHT)
button4=Button(root,text="-MONEY WITHDRAWAL-",command=crow)
button4.pack(side=RIGHT)
button5=Button(root,text="-SAVING ACCOUNT DETAILS-")
button5.pack(side=RIGHT)
button6=Button(root,text="-DEPOSIT-",command=moo)
button6.pack(side=RIGHT)

def custombox_quit():
    answer=tkinter.messagebox.showinfo("---WARNING---","Are you sure you want to cancel?")
    if answer:
        root.destroy()
button8=Button(root,text="---EXIT---",fg="red",bg="yellow",command=custombox_quit)
button8.pack(side=LEFT)
def myinfo():
    root6=Tk()
    root6.title("INFO")
    label_info=Label(root6,text="PESU BANK\n CHAIRMAN Mr  ROHIT VISHWAKARMA \n VICE CHAIRMAN Mr B SHANKAR \n CONTACT:-9880218337")
    label_info.pack(side=LEFT)
    label_info1=Label(root6,text="A GOVERNMENT OF INDIA UNDERTAKING",fg="white",bg="black")
    label_info1.pack(side=TOP)
    root6.mainloop()
button9=Button(root,text="INFO",fg="green",bg="white",command=myinfo)
button9.pack(side=BOTTOM)                        
status=Label(root,text="Running >>>.... -by ROHIT VISHWAKARMA,PES1201800152------",relief =SUNKEN,anchor=W,bd=1)
status.pack(side=BOTTOM,fill=X)
button10=Button(root,text="other SERVICES..",fg="indigo",command=service)
button10.pack()
button11=Button(root,text="SECURITY",fg="green",bg="white",command=security)
button11.pack(side=BOTTOM)
root.mainloop()





