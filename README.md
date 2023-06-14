# Extrovert-vs.-Introvert-Game
Have you ever been asked, "Are you an extrovert or an introvert?"

     def percentage_calculation(score, total):
          return (score / total) * 100
     def Extrovert_Introvert_Game():

    name = input("Enter your name: ")
    intro = f"Hello, {name}! Thank you for playing this game. Please answer the following, as honestly as possible to get the most accurate results."
    print(intro)
    questions = ["Scenario 1: You just finished taking your last exam of the year and have free time. It's still pretty early in the day so you are contemplating on what to do now. Would you rather (A) Celebrate/Hang out with your friends or (B) Stay at home and chill by yourself (watch a movie, read, sleep, etc...)",
                "Scenario 2: You and your friends decide to go out and eat. After looking through the menu, you all agree on what orders/foods you want to share. However, someone has to go up to call the waiter and tell them your order. Are you the friend who (A) Waves at the waiter and places the order for everyone or (B) Waves at the waiter but let'Ssomeone someone else place the order",
                "Scenario 3: You and your friend decide to have a picnic at the park. While you are setting up your blanket on the grass, a lady suddenly comes along and tells you she was going to have her picnic there. You were there first, but this lady is lowkey a Karen and is making a scene in front of everyone. Will you (A) Stand your ground, and tell her to look for another spot since you and your friend were there first or (B) Decide it's best to give up the spot to her so you do not make a bigger scene",
                "Scenario 4: You go to the store to buy an item you need. You spend a good 10 minutes trying to find the item on the shelf but have no luck. Do you (A) Look for an employee and ask for assistance or (B) Keep looking by yourself until you ultimately give up and come to the conclusion that the item is not in stock, and decide to come another day.",
                "Scenario 5: Your dad/mom is giving you a ride to a concert, but they've been waiting for you in the car for 10 minutes already. You rush to get ready and run out of the house to get in the car before they get even more upset. However, five minutes later, you realized you forgot your ID at home. Will you (A) Tell your dad/mom that you forgot something at home and ask if they can go back or (B) Keep quiet and pray for the best because you don't want them to get upset",    
                "Scenario 6: You're in math class and the teacher puts a problem on the board. The teacher asks if anyone knows the answer. When you look at the problem you realize that you know how to solve it. The teacher says that they will not move on until someone speaks up, however, no one moves and then there is complete silence. Do you (A) Raise your hand and attempt to answer or (B) Stay quiet because someone else will eventually speak up.",]
    extrovert_score = 0
    introvert_score = 0
    for question in questions:
        print(question)
        response = input("Pick (A) or (B): ")
        if response == "A" or response == "a":
            extrovert_score += 1
        elif response == "B" or response == "b":
            introvert_score += 1
        else:
            print ("Invalid response!")
    total_questions = 6
    extrovert_percentage = percentage_calculation(introvert_score, total_questions)
    introvert_percentage = percentage_calculation(extrovert_score, total_questions)
    print("Calculating your results...")
    print("Extrovert percentage: {:2f}%".format(extrovert_percentage))
    print("Introvert percentage: {:2f}%".format(introvert_percentage))

    
