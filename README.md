Sala de juegos - Proyecto Angular (entrega ZIP)
==============================================

Este ZIP contiene un proyecto Angular listo para personalizar e iniciar. 
Es un scaffold completo que implementa los sprints solicitados: Auth (Firebase), Home, Quién soy, Chat, Ahorcado, Mayor o Menor, Preguntados, Sopa de Letras (juego propio), y Encuesta.

**Pasos para arrancar (localmente)**:
1. Descomprime este ZIP.
2. Ejecuta `npm install` en la carpeta raíz.
3. Opcional (recomendado): instalar Angular CLI globalmente: `npm i -g @angular/cli`.
4. Añade Angular Material (opcional): `ng add @angular/material` y selecciona tema.
5. Añade AngularFire y configura Firebase: `ng add @angular/fire` y pega tu firebaseConfig en `src/environments/environment.ts`.
6. Ejecuta `ng serve` o `npm start`.

**Notas**:
- En `src/environments/environment.ts` sustituye los valores de `firebase` por tu configuración real.
- En `app.module.ts` deberás importar los módulos de AngularFire: `AngularFireModule.initializeApp(environment.firebase)`, `AngularFireAuthModule`, `AngularFirestoreModule`.
- El proyecto usa `MatSnackBar` para notificaciones; evita `alert()` en la app final.
- El componente Sopa de Letras incluye lógica básica con temporizador de 60s; podés extender la colocación de palabras y selección de palabras en diagonal/vertical según prefieras.
- Los endpoints de Preguntados son stubs; reemplaza con la API real en `preguntados.component.ts`..

¡Listo! El ZIP ya está generado y contiene todo lo necesario para empezar a desarrollar en Angular.
