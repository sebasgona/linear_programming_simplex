function [xo, zo, ban, iter] = mSimplexFaseII(A, b, c)
% purpose: Version del Simplex en la Fase II
% minimizar c^T x
% sujeto a Ax <= b , x >= 0 , b >= 0
%
% In : 
% A ... mxn matrix
% b ... column vector with as many rows as A
% c ... column vector with as many entries as one row of A
%
% Out: xo ... SFB  optima del problema
% zo ... valor  optimo del problema
% ban ... indica casos:
% -1 ... si el conjunto factible es vacio
% 0 ... si se encontro una solucion  optima
% 1 ... si la funci on objectivo no es acotada.
% iter ... es el numero de iteraciones (cambios de variables basicas)
% que hizo el metodo
%

size_b = size(b);
costos = [-c  zeros(size_b)];
B = [ zeros(size(c)) ones(size_b)];
M = [A eye(size_b(2))];

iter_count = 0;
next_step = 1;
band = 0;

while next_step && band ~= -1
    iter_count = iter_count + 1;
    x_out = max(costos);
    x_out_index = find(costos == max(costos));
   
    h = M(:,x_out_index);
   
    if  all(h <= 0) == 1
        band = -1
        %Agregar codigo para caso degenerad
    end
    
    min_vector = b'./h;
    
    x_in = min(min_vector)
    x_in_index = find(min_vector == min(min_vector))
    
    if 
    
    break
end

end

 