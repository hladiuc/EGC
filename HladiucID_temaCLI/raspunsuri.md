1. Ce este un viewport?
    Viewport-ul este zona de vizibila a unei scene(ce vedem).

2. Ce reprezintă conceptul de frames per seconds din punctul de vedere al bibliotecii OpenGL?
    Numarul de cadre randate pe secunda

3. Când este rulată metoda OnUpdateFrame()?
    Este rulata inainte de OnRenderFrame() si este necesara pentru a actualiza logica aplicatiei (ex. miscarea obiectelor)

4. Ce este modul imediat de randare?
    Modul imediat randeaza obiectele fara a le stoca in memoria GPU pentru utilizari ulterioare.

5. Care este ultima versiune de OpenGL care acceptă modul imediat?
    Modul imediat a fost marcat ca "deprecated" in OpenGL 3.0 si eliminat in OpenGL 3.1.

6. Când este rulată metoda OnRenderFrame()?
    Este rulata dupa OnUpdateFrame()

7. De ce este nevoie ca metoda OnResize() să fie executată cel puțin o dată?
    Latimea si inaltimea initiale sunt 0, apoi face resize la setarile aplicatiei.

8. Ce reprezintă parametrii metodei CreatePerspectiveFieldOfView() și care este domeniul de valori pentru aceștia?
    Parametri :
    - fieldOfView : unghiul camerei pe axa OY , cuprins intre 0 si PI(180 grade)
    - aspectRatio : raport latime si inaltime
    - nearPlaneDistance : distanta minima de vizualizare a scenei
    - farPlaneDistance : distanta maxima de vizualizare a scenei