import os
from Board import Board

board = Board()


def print_header():
    print("Welcome\n")


def refresh_screen():
    os.system("cls")
    print_header()
    board.display()


while True:
    refresh_screen()
    x_choice = int(input("\nX) Enter chooice  1 - 9 >>>"))
    board.update_cell(x_choice, "X")
    refresh_screen()
    if board.is_winner("X"):
        print("\nX wins!!!\n")
        play_again = input("Wanna play again?(Y/N)>>").upper()
        if play_again == "Y":
            board.reset()
            continue
        else:
            break
    if board.is_tie():
        print("\nTie game!!!\n")
        play_again = input("Wanna play again?(Y/N)>>").upper()
        if play_again == "Y":
            board.reset()
            continue
        else:
            break
    o_choice = int(input("\nO) Enter chooice  1 - 9 >>>"))
    board.update_cell(o_choice, "O")
    if board.is_winner("O"):
        print("\nO wins!!!\n")
        play_again = input("Wanna play again?(Y/N)>>").upper()
        if play_again == "Y":
            board.reset()
            continue
        else:
            break
    if board.is_tie():
        print("\nTie game!!!\n")
        play_again = input("Wanna play again?(Y/N)>>").upper()
        if play_again == "Y":
            board.reset()
            continue
        else:
            break
