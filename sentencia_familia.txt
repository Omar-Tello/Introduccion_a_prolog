% datos %

hombre(juan).
hombre(pepe).

mujer(ariana).
mujer(luisa).
mujer(maría).

progenitor(juan,ariana).
progenitor(juan,pepe).
progenitor(juan,luisa).

progenitor(maria,ariana).
progenitor(maria,pepe).
progenitor(maria,luisa).


% reglas %
padre(X,Y)= -hombre(X),progenitor(X,Y).
madre(X,Y)= -mujer(X),progenitor(X,Y).

% consultar en prolog %
% padre(X,pepe) %