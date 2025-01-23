Condução bidimensional sem geração de calor. Para resolver um problema bidimensional, basta não incluir as fronteiras na direção a ser ignorada no campo `boundary` no arquivo `blockMeshDict`. As faces de fronteira assim ignoradas receberão automaticamente o tipo `empty`. O mesmo é válido para configurar problemas unidimensionais.

Condição inicial:

$$T=273$$

Condições de contorno:

$$\begin{align}
x=0: \qquad &\frac{\partial T}{\partial x}=0\\
x=1: \qquad &T=500\\
y=0: \qquad &\frac{\partial T}{\partial y}=0\\
y=1: \qquad &\frac{\partial T}{\partial y}=0
\end{align}$$
