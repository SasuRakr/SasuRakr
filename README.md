while True:
    import random

    a= int(input("Enter the lower Limit number:-"))
    b= int(input("Enter the upper Limit number:-"))
    random_number = random.randint(a,b)
    n=int(input("Enter the total number of Chances you want \n"))
    count = 0
    while count<3:
        guess = int(input("Enter the number you guessed \n"))
        count +=1
        if guess==random_number:
            print(f"Guessed NUmber is {guess} and the Random NUmber is {random_number}")
            print("Badhai Xa")
            break
        elif guess<random_number:
            print("Guessed Number is Less")
        elif guess>random_number:
            print("Guessed NUmber is too large")
        if count==n:
            print("Your Chances are Finished")
            print("The Correct Number is",random_number)
            break
    print("\n")
    break


