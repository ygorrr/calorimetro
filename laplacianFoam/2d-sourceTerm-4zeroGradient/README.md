Condução bidimensional com geração de calor. Para resolver um problema bidimensional, basta não incluir as fronteiras na direção a ser ignorada no campo `boundary` no arquivo `blockMeshDict`. As faces de fronteira assim ignoradas receberão automaticamente o tipo `empty`. O mesmo é válido para configurar problemas unidimensionais.

O solver `laplacianFoam` oferece suporte a termos fonte/sumidouro, os quais são implementados através do objeto `fvOptions(T)` no código fonte. Caso não exista, crie o arquivo `fvOptions` na pasta `system` do caso e lá defina o termo a ser modelado.


Condição inicial:

$$T=0$$

Condições de contorno:

$$\begin{align}
x=0: \qquad &\frac{\partial T}{\partial x}=0\\
x=1: \qquad &\frac{\partial T}{\partial x}=0\
y=0: \qquad &\frac{\partial T}{\partial y}=0\\
y=1: \qquad &\frac{\partial T}{\partial y}=0
\end{align}$$
