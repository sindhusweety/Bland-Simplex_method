# Bland-Simplex_method


INPUT:

```self.equations = ['x_1 + x_2 <= 6', 'x_1 - x_2 <= 0']
self.obj_atrributes = [36, 30, -3, -4]       #[5, 2] #an array of objective function coefficients----------5x_1 + 2x_2
self.decision_variable_rhs=[5, 10]   #[6, 0] # right-hand side entries
self.decision_variable_lhs = [[1, 1, -1, 0], [6, 5, 0, -1]] #[[1, 1],[1, -1 ]] #coefficients for the left-hand-sides of the constraints
self.no_equations = len(self.decision_variable_lhs)
self.no_variables = len(self.decision_variable_lhs[0])
self.lowbound = "x1, x2 >= 0"
```




OUTPUT:

```--------------------------------------------------------------------------
L.H.S of Objective Function"s Coefficients  [1, -36, -30, 3, 4, 0, 0]
R.H.S : [0, 5, 10]
Initial Basic Variables  ['s_1', 's_2']
L.H.S of Constraints" Coefficients :  [[0, 1, 1, -1, 0, 1, 0], [0, 6, 5, 0, -1, 0, 1]]
Basic Variables  ['s_1', 's_2']
Variables are  ['z', 'x_1', 'x_2', 'x_3', 'x_4', 's_1', 's_2']
table columns : ['z', 'x_1', 'x_2', 'x_3', 'x_4', 's_1', 's_2', 'rhs', 'BV']
---------------------------------------------------------------------------
Initial Stage ...
   z  x_1  x_2  x_3  x_4  s_1  s_2  rhs   BV
0  1  -36  -30    3    4    0    0    0    z
1  0    1    1   -1    0    1    0    5  s_1
2  0    6    5    0   -1    0    1   10  s_2
------------------------------------------------------------------------------------
------------------------------------------------------------------------------------
     z  x_1       x_2  x_3       x_4  s_1       s_2    rhs   BV
0  1.0  0.0  0.000000  3.0 -2.000000  0.0  6.000000  60.12    z
1  0.0  0.0  0.166667 -1.0  0.166667  1.0 -0.166667   3.33  s_1
2  0.0  1.0  0.833333  0.0 -0.166667  0.0  0.166667   1.67  x_1
------------------------------------------------------------------------------------
------------------------------------------------------------------------------------
------------------------------------------------------------------------------------
     z  x_1  x_2  x_3  x_4   s_1  s_2     rhs   BV
0  1.0  0.0  2.0 -9.0  0.0  12.0  4.0  100.08    z
1  0.0  0.0  1.0 -6.0  1.0   6.0 -1.0   19.98  x_4
2  0.0  1.0  1.0 -1.0  0.0   1.0  0.0    5.00  x_1
------------------------------------------------------------------------------------
------------------------------------------------------------------------------------
Final Output
------------------------------------------------------------------------------------
UNBOUNDED LP
     z  x_1  x_2  x_3  x_4   s_1  s_2     rhs   BV
0  1.0  0.0  2.0 -9.0  0.0  12.0  4.0  100.08    z
1  0.0  0.0  1.0 -6.0  1.0   6.0 -1.0   19.98  x_4
2  0.0  1.0  1.0 -1.0  0.0   1.0  0.0    5.00  x_1
```

