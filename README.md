email1= input("Enter your Email:")
k=0
j=0
d=0
if len(email1)>=6:
    if email1[0].isalpha():
        if ("@" in email1) and (email1.count("@")==1):
            if (email1[-4] == ".") ^ (email1[-3]=="."):
                for i in email1:
                    if i==i.isspace():
                        k=1
                    elif i.isalpha():
                        if i==i.upper():
                            j=1

                    elif i.isdigit():
                        continue
                    elif i=="_" or i=="." or i=="@":
                        continue
                    else:
                        d= 1


                if k==1 or j==1 or d==1:
                    print("Wronge Email 5")
                else:
                    print("Right Email")
            else:
                print("wronge Email 4")
        else:
            print("wronge Email 3")
    else:
        print("wronge Email 2")
else:
    print("wronge Email 1")# emailvalidition
we can check our email is right or wronge
