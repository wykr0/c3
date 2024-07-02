# certamen #3 Manuel Cruces

Para poder ejecutar, debe instalar las librerías necesarias:

```
npm install
npm install supertest
npm install jest
npm install sinon

```

Finalmente ejecutar el script de tests:

```
npm run test
```

El script de test definido en el archivo `package.json` tiene el siguiente comando:

```
jest --runInBand
```

La opción `--runInBand` permite correr los tests uno después del otro, y eso evita el problema al levantar
el servidor en un determinado puerto, puesto que cada test lo intenta hacer, y si encuentra que el
puerto ya se está usando, los tests se van a caer.
