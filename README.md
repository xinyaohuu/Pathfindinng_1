# Topic: Using gpt4 api to solve the following question

A {x} * {y} grid map with {(x)*(y)} blue dots(with x from 0 to {x} and y from 0 to {y}) representing coordinates and lines connecting them. Each adjacent coordinate is connected by a blue straight line, either horizontally or vertically, and the distance of 1. The grid starts from (0,0) at the bottom left and goes up to {x-1} * {y-1} at the top right. Obstacles on the grid are represented by the absence of blue dots at specific coordinates, as well as the missing adjacent blue lines connecting them. The coordinates with obstacles are:(obs_coordinates) with x and y from 0 to {x-1}, corresponding to the coordinate system. Thus, I need to find the shortest path from (0,0)to {x-1} * {y-1} to solve this problem you are required 1. moving each step either horizontally or vertically and avoiding obstacles by distance of 1. 2. don't recap the problem, please get straight to solve it 3. you will get the history of this problem which you did before 4. only need text-based path coordinates results "


# Step 1: Generate random obstacles
  1. Due to small mapsize, percentage of obstacles are indentical, so we can manully delete those rows

  2. Grid size: 3*3 to 11*11,Percentage of obstacles: 0%, 5%, 10%, 15%, 20%, 25%, Number of groups: 10 for each percentage

# Step 2: Use Dijkstra and astar to find the shortest path

# Step 3: Use gpt4 api to find the shortest path 

# Step 4: Format the gpt4 output: complete output and summary output

# Step 5: Check if gpt4 answer is the shortest path
    1. length should be equal to the length of Dijkstra 
    2. Bypass the obstacles
    3. Start coordinate and end coordinate should be (0,0) and (x-1,y-1)
    3. Each step should be 1