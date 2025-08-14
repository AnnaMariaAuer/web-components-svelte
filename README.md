# Publish einer neuen Version

Beispiel: neue Version taggen und dann pushen: Paket wirt automatisch gebaut und veröffentlicht.
Version muss in package.json angepasst werden.

```
git tag v1.0.0
git push origin v1.0.0
```

## Installation in einer anderen App

.npmrc-File, das nicht gepusht wird. Alternative: GitHub Actions Flow

```
//npm.pkg.github.com/:_authToken=${NODE_AUTH}
@AnnaMariaAuer:registry=https://npm.pkg.github.com
```

## Color-Scheme überschreiben

Die Komponenten arbeiten mit CSS-Variablen. Diese können in der Consumer-App entsprechend überschrieben werden:

```
:root {
	--primary-color: #ff0;
	--color-on-primary: #000;
	--secondary-color: #cf3476;
	--focus-outline: #feff7a;
}
```
