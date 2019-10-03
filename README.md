# ENPM-809Y-Introduction-to-Robot-Programming
This is a C++ and ROS based course.
## Assignment 1

1. Create a 2D array of std::string with 3 rows and 2 columns

2. Initialize the array to have the following elements

  &nbsp; &nbsp; &nbsp; &nbsp; ◦First row:blue,white

  &nbsp; &nbsp; &nbsp; &nbsp; ◦Second row:green,white

  &nbsp; &nbsp; &nbsp; &nbsp; ◦Third row:green,white 

3. Create 3 std::stringvectors (color_vec1,color_vec2, andcolor_vec3), each representing a row of pegs. 

4. Read the 2D array and store values of each row in a vector

   &nbsp; &nbsp; &nbsp; &nbsp; ◦color_vec1: First row of the array

   &nbsp; &nbsp; &nbsp; &nbsp; ◦color_vec2: Second row of the array

   &nbsp; &nbsp; &nbsp; &nbsp; ◦color_vec3: Third row of the array

5. Prompt the user to enter the color for the missing peg usingthe picture of the tray

   &nbsp; &nbsp; &nbsp; &nbsp; ◦Only 1cout: The user should enter the three colors on the sameline◦The user should enter:green white blue.

6 Appropriately insert the first, second, and third input incolor_vec1,color_vec2, andcolor_vec3, respectively

   &nbsp; &nbsp; &nbsp; &nbsp; ◦Make sure to insert these inputs at the right place in each vector7.

7.Display the elements of each vector in the console (1stelement,2ndelement, and3r delement).
  Output should be:

   &nbsp; &nbsp; &nbsp; &nbsp; Vector 1: blue white green
   
   &nbsp; &nbsp; &nbsp; &nbsp; Vector 2: white green white
   
   &nbsp; &nbsp; &nbsp; &nbsp; Vector 3: green blue white

8. Create a 2D vector (3 rows and 3 columns) of std::stringnamedcolor_vec_2d.

9. Use color_vec1,color_vec2, and color_vec3 to buildcolor_vec_2d

    &nbsp; &nbsp; &nbsp; &nbsp; ◦First row ofcolor_vec_2dconsists of elements of color_vec1

    &nbsp; &nbsp; &nbsp; &nbsp; ◦Second row ofcolor_vec_2dconsists of elements of color_vec2

    &nbsp; &nbsp; &nbsp; &nbsp; ◦Third row ofcolor_vec_2dconsists of elements of color_vec3

10. Display the size ofcolor_vec_2d

11. Read and displaycolor_vec_2din the console. The output should be:
   &nbsp; &nbsp; &nbsp; &nbsp; blue    white   green
   
   &nbsp; &nbsp; &nbsp; &nbsp; white   green   white
   
   &nbsp; &nbsp; &nbsp; &nbsp; green   blue    white
