Markdown

# Transportation Problem Solver

A Java-based GUI application for solving transportation problems using the Vogel's Approximation Method (VAM) for initial basic feasible solutions and the Stepping Stone Method for optimality testing and improvement. This tool helps in minimizing transportation costs from multiple sources to multiple destinations.

## ✨ Features

* **Interactive GUI:** Built with `swing` for a user-friendly experience.

* **Dynamic Input:** Allows users to specify the number of sources and destinations, then input custom cost matrices, supply values, and demand values.

* **Vogel's Approximation Method (VAM):** Implements VAM to find an efficient initial basic feasible solution.

* **Stepping Stone Method:** Applies the Stepping Stone Method to check for optimality and iteratively improve the solution by identifying and utilizing closed paths with negative costs.

* **Total Cost Calculation:** Accurately calculates the minimum total transportation cost.

* **Allocation Display:** Shows the optimal allocation of units from sources to destinations.


## 🚀 How to Use

### Prerequisites

- **Java 8 or above** installed  
- A Java IDE like **IntelliJ IDEA**, **Eclipse**, or **NetBeans**  


### Running the Application

1. **Save the code:** Save the provided Python code as `transportation_solver.java`.



3. **Execute:** Run the script from your terminal:

javac TransportationSolver.java
java TransportationSolver

### Application Flow

1. **Initial Screen:** The application will start in fullscreen mode. Press any key to proceed.

2. **Input Dimensions:** Enter the number of sources (rows) and destinations (columns) in the respective fields and click "Generate".

3. **Cost Matrix Input:** A new screen will appear where you can input the cost for transporting one unit from each source to each destination. Click "NEXT".

4. **Supply and Demand Input:** On the final input screen, enter the supply available at each source and the demand required at each destination.

5. **Solve:** Click the "Solve" button. The application will calculate the optimal transportation plan and display the total minimum cost. A truck animation will then play to signify the completion of the transportation.

## ⚙️ Core Algorithms

This project implements two fundamental algorithms in operations research for solving transportation problems:

### 1. Vogel's Approximation Method (VAM)

VAM is used to find a good initial basic feasible solution. It works by calculating "penalties" for each row and column (the difference between the two lowest costs) and then allocating units to the cell with the highest penalty, aiming to minimize the initial cost.

### 2. Stepping Stone Method

The Stepping Stone Method is an iterative procedure used to test the optimality of an initial basic feasible solution obtained from methods like VAM. It identifies "closed paths" (loops) involving empty cells and allocated cells. If a closed path results in a negative cost reduction, units are reallocated along that path to decrease the total transportation cost until no further improvements can be made.

## 🤝 Contributing

Contributions are welcome! If you have suggestions for improvements, bug fixes, or new features, please feel free to:

1. Fork the repository.

2. Create a new branch (`git checkout -b feature/YourFeature`).

3. Make your changes.

4. Commit your changes (`git commit -m 'Add some feature'`).

5. Push to the branch (`git push origin feature/YourFeature`).

6. Open a Pull Request.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

**Note:** Remember to replace `truck.png` and `1st.jpg` with your actual image files or update the code to use placeholder images if you don't have them.