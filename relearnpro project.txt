def main():
    
    qs={'sein ':'to be', 'haben ':'to have', 'werden ':'to become', 'sagen ':'to say', 'geben ':'to give'}
    print("*** Quiz ***\n")
    name = input("Please enter your name: ").title()
    print()
    print("\nWell done {0}, you scored {1} out of {2}.".format(name, quiz(qs), len(qs)))
def quiz(qs):
    score = 0
    for q,a in qs.items():
        if input(q).lower() == a.lower():
            score += 1
            print("Correct.")
        else:
            print("Sorry, correct answer is \"{}\".".format(a))
            return score
 
if __name__ == "__main__":
    main()