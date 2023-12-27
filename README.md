# games
# coming soon @star1608 i want to say thank you to my teacher for everything you are the best
class Colors:
    RESET = '\033[0m'
    RED = '\033[91m'
    GREEN = '\033[92m'
    YELLOW = '\033[93m'
    BLUE = '\033[94m'

def start():
    print("==========================================")
    print("           " + f"{Colors.YELLOW}Welcome to Amir games{Colors.RESET}")
    print("==========================================")

def menu():
    print("Welcome to my game. In this game, you will be able to choose a few games:")
    print(f"{Colors.RED}1: Guess the number from 1-10{Colors.RESET}")
    print(f"{Colors.BLUE}2: Your average of 3 last exams{Colors.RESET}")
    print(f"{Colors.GREEN}3: Hangman game{Colors.RESET}")
    user_choice = input("Enter the game you want to play: ")

    if user_choice == "1":
        import main3
    elif user_choice == "2":
        import main
    elif user_choice == "3":
        import fun
    else:
        print("Sorry, I don't have this choice available")

def main():
    start()
    menu()

if __name__ == '__main__':
    main()
