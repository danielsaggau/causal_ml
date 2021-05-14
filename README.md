# A Gentle Introduction into SCM 

Repo for essay on structural causal models 


 | Association-based Concepts |  Causal Concepts
|--------------------------|------------------------|
| Correlation              | Randomization  
| Regression               | Confounding
| Conditional Independence | Disturbance
| Likelihood               | Error Terms      
| Odds Ratio               | Structural Coefficients       
| Propensity Score         | Spurious Correlation    

Table: Concepts in Causality and Association concepts

## Pearl Causal Hierachy 

 |Method         | CBN |  SCM
|----------------|---------------------------|------------------------|
| Prediction     | $\boldsymbol{\cdot}$ Unstable                                                                                        | $\boldsymbol{\cdot}$ Stable                 
|                | $\boldsymbol{\cdot}$ Volatile to parameter changes                                                                   | $\boldsymbol{\cdot}$ More Natural Specification 
|                | $\boldsymbol{\cdot}$ Re-Estimate entire model                                                                        | $\boldsymbol{\cdot}$ Only estimate $\Delta$ CM
|                |                                                                                                                      | 
| Intervention   | $\boldsymbol{\cdot}$ Costly for Non-Markovian Models                                                                 | $\boldsymbol{\cdot}$ Pot. Cyclic Representation
|                | $\boldsymbol{\cdot}$ Unstable(Nature CP)                                                                             | $\boldsymbol{\cdot}$ Stable(Nature Eq.)
|                | $\boldsymbol{\cdot}$ Only generic estimates($\Delta$ CP)                                                             | $\boldsymbol{\cdot}$ Context specific(Invariance of Eq.)
|                |                                                                                                                      | 
|Counterfactuals | $\boldsymbol{\cdot}$ **Impossible**                                                                                  | $\boldsymbol{\cdot}$ Possible
|                | $\boldsymbol{\cdot}$ no information on latent factors($\epsilon$)                                                    | $\boldsymbol{\cdot}$ Inclusion of latent factors


## Causal Inference and Time 

\begin{array}{|l|l|l|l|l|l|}
\hline \text { model } & \begin{array}{l}
\text { predict in IID } \\
\text { setting }
\end{array} & \begin{array}{l}
\text { predict under } \\
\text { changing } \\
\text { distributions / } \\
\text { interventions }
\end{array} & \begin{array}{l}
\text { answer } \\
\text { counter- } \\
\text { factual } \\
\text { questions }
\end{array} & \begin{array}{l}
\text { obtain } \\
\text { physical } \\
\text { insight }
\end{array} & \begin{array}{l}
\text { automatically } \\
\text { learn from } \\
\text { data }
\end{array} \\
\hline \begin{array}{l}
\text { mechanistic } \\
\text { model } \\
\end{array} & \mathrm{Y} & \mathrm{Y} & \mathrm{Y} & \mathrm{Y} & ? \\
\hline \begin{array}{l}
\text { structural } \\
\text { causal model }
\end{array} & \mathrm{Y} & \mathrm{Y} & \mathrm{Y} & \mathrm{N} & \mathrm{Y} ? ? \\
\hline \begin{array}{l}
\text { causal } \\
\text { graphical } \\
\text { model }
\end{array} & \mathrm{Y} & \mathrm{Y} & \mathrm{N} & \mathrm{N} & \mathrm{Y} ? \\
\hline \begin{array}{l}
\text { statistical } \\
\text { model }
\end{array} & \mathrm{Y} & \mathrm{N} & \mathrm{N} & \mathrm{N} & \mathrm{Y} \\
\hline
\end{array}

