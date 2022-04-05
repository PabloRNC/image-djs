# 🎨 Image DJS

> ¡Un generador de imágenes para discord.js!

## Ejemplos

### Welcome

```javascript
const { Welcomer } = require('image-djs');
// typescript: import { Welcomer } from 'image-djs';
const file = await new Welcomer()
	.setAvatar('https://c.tenor.com/bMJ1lh3r46gAAAAC/pfp.gif')
	.setBackground('https://i.pinimg.com/736x/33/75/00/33750046310a78fc55914a621c7e0991.jpg')
	.setBorderColor('#ababab')
	.setAvatarBorderColor('#ff4546')
	// .setUserFont('52px "Segoe UI"') | Debes cargar una fuente personalizada con canvas
	// .setSubtitleFont('32px "Segoe UI"') | Debes cargar una fuente personalizada con canvas
	.setSubtitle('Bienvenido!')
	.setUsername('drgato')
	.build(true, 'welcomer-xd.png');

channel.send({ files: [file] });
```

#### Ejemplo:

<img src="https://i.imgur.com/Fa0aWlt.png" height="200px"/>

### Ping

```javascript
const { Ping } = require('image-djs');
// typescript: import { Ping } from 'image-djs';
const file = await new Ping()
	.setIcon('https://i1.sndcdn.com/avatars-twM1pq6gSk4YzN4F-N4zKuw-t500x500.jpg')
	.build(true, 'ping.png');

channel.send({ files: [file] });
```

#### Ejemplo:

<img src="https://i.imgur.com/zkqoQ3w.png" height="200px"/>

> ⚠️ Próximamente más clases... Reporta los bugs en el [GitHub](https://github.com/drgatoxd/image-djs/issues) del npm.
