# BD-FIB
Resumen para el examen final de la asignatura de Base de Datos de la FIB

Àlgebra relacional
Cal que T i S siguin relacions compatibles (tenen esquemes amb un conjunt d’atributs idèntic, i els dominis de cada parella d’atributs són els mateixos a T i a S)=
-UNIÓ
R =PERSONAL-ADM  PERSONAL-LAB
-INTERSECCIÓ
R =PERSONAL-ADM  PERSONAL-LAB
-DIFERENCIA
R =PERSONAL-ADM − PERSONAL-LAB
No fa falta que siguin compatibles=
-PRODUCTE CARTESIÁ
R =MODUL-CN  OFICINA
-REANOMAMENT
R =PERSONAL-DOC {modul-de -> modul, num-de -> num}
-SELECCIÓ
R =OFICINA(modul-de=‘B2’ AND superfície>16)
-PROJECCIÓ
R =PERSONAL-ADM[modul, num]
-COMBINACIÓ
R =MODUL-CN[modul=modul-de]OFICINA
R =MODUL-CN[modul=modul-de, sup-promig-of=superfície]OFICINA
-NATURAL JOIN
R =PERSONAL-ADM[modul*modul-de, num*num-de]OFICINA
R =PERSONAL-ADM * MODUL-CN

# Model relacional
Fila = Tupla
Columna = Atribut
Cardinalitat d’una relació: Es el nombre de tuples de la
