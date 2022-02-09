_Please stick to the headings and their order. Don't modify the words in bold. Your input is required at each occurrence of "e.g." and "..."._<br>
_You may use https://tex-image-link-generator.herokuapp.com/ to render math formulas in Markdown, see the examples below._

## Physics

### PDEs

One mass balance per each phase; CO2 gas phase and aqueous phase.
One solute transport of CO2 dissolved in aqueous phase.

### Constitutive relations

#### Fluid-matrix interaction

* **Capillary pressure:** Brooks-Corey
  ![p_c(S_{l}) = p_\text{entry}S_{le}^{-1/\lambda}](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+p_c%28S_%7Bl%7D%29+%3D+p_%5Ctext%7Bentry%7DS_%7Ble%7D%5E%7B-1%2F%5Clambda%7D%0A)

* **Relative permeability:** Brooks-Corey ![k_{rw} = (\frac{S_w - S_{wr}}{1 - S_{wr}})^{\frac{2 + 3\lambda}{\lambda}}](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+k_%7Brw%7D+%3D+%28%5Cfrac%7BS_w+-+S_%7Bwr%7D%7D%7B1+-+S_%7Bwr%7D%7D%29%5E%7B%5Cfrac%7B2+%2B+3%5Clambda%7D%7B%5Clambda%7D%7D) , 
 ![k_{rco_2} = (\frac{1 - S_w}{1 - S_{wr}}) [1 - (\frac{S_w - S_{wr}}{1 - S_{wr}})^{\frac{2 + \lambda}{\lambda}}]](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+k_%7Brco_2%7D+%3D+%28%5Cfrac%7B1+-+S_w%7D%7B1+-+S_%7Bwr%7D%7D%29+%5B1+-+%28%5Cfrac%7BS_w+-+S_%7Bwr%7D%7D%7B1+-+S_%7Bwr%7D%7D%29%5E%7B%5Cfrac%7B2+%2B+%5Clambda%7D%7B%5Clambda%7D%7D%5D) 

#### Phase composition: Applied equations of state

* **CO2 in liquid phase:** ...

* **Water in gas phase:** ...

#### Density

* **Liquid phase:** ...

* **Gas phase:** ...

### Spatial parameters

_Please provide the relevant facies parameters as a csv file._<br>
_E.g._ The parameters ![p_\text{entry}, \lambda, S_{lr}, S_{gr}](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+p_%5Ctext%7Bentry%7D%2C+%5Clambda%2C+S_%7Blr%7D%2C+S_%7Bgr%7D%0A) for the different facies are given in [spatial_parameters.csv](spatial_parameters.csv).<br>
_Obviously, the number and type of parameters for your model might differ from the ones in the provided template._

## Numerics

### Coupling of flow and transport, temporal and spatial discretization

_E.g._ Fully coupled, fully implicit, cell-centered FV with TPFA.

### Linearization and Solvers

_E.g._ Newton with line search, AMG-preconditioned BiCGSTAB for the linear systems.

### Primary Variables

_E.g._ Dependent on local phase composition:
* Both phases present:
  ![p_l, S_g](https://render.githubusercontent.com/render/math?math=%5Ctextstyle+p_l%2C+S_g%0A)...
