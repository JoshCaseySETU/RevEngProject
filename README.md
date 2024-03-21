# Swapcase Assembly Program

## Author
Josh Casey

## Student Number
C00261828

## License
This project is licensed under the GNU General Public License v3.0 (https://www.gnu.org/licenses/gpl-3.0.en.html#license-text). 

## Project Description
The project was designed to preform a case swap on a string no larger than 23 characters. i.e THIS IS wild! - this is WILD!
The case swapping function, works by comparing each characters ascii value with the value of a-z & A-Z, ensuring it is an alphanumoric character. 
Depending on if the character is between a-z or A-Z it will then add or substract 32 from the ascii value to get its corrosponding case size.  

## Instructions for Producing an Executable
1. Make sure NASM (The Netwide Assembler) is installed on your Linux system.
2. Open a terminal and navigate to the directory containing the assembly program.
3. Run the following commands to assemble and link the program:
    ```bash
    nasm -f elf64 swapcase.asm -o swapcase.o
    ld swapcase.o -o swapcase
    ```
4. Once the executable is generated, you can run it by executing the following command:
    ```bash
    ./swapcase
    ```
5. Follow the on-screen instructions to input a string and see the swapcase result.

## Issues/Notes
- This program assumes that the input string contains only ASCII characters. Non-ASCII characters may not be handled correctly.
- Ensure that you have appropriate permissions to execute the generated binary file.
