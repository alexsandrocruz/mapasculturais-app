## Mapas Culturais APP

    < Mapas Culturais Cross-plataform IONIC APP >
    Copyright (C) <2016> <Instituto TIM>

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.

    You should have received a copy of the GNU Affero General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
    
---

Este é o repositório do aplicativo Android do sistema [Mapas Culturais](https://github.com/hacklabr/mapasculturais). Ele é orientado para funcionar como uma espécie de Agenda Cultural. Entre suas principais funcionalidades, estão:

* Apresentar uma consulta dos dados (Eventos, Espaços, Agentes, Projetos) de todas as instâncias vigentes do Mapas Culturais; 
* Permitir a seleção manual de uma determinada instalação;
* Exibir geolocalização do mapa a partir da instalação mais proxima, pela localização do gps do mobile device;


# Download e build
------------------

Se você já tem o npm instalado, basta fazer:

* Instalar o ionic globalmente
```
$ sudo npm -g install cordova ionic bower
```

* Clonar o repositório
```
$ git clone https://github.com/hacklabr/mapasculturais-app.git
```

* Fazer o build padrão
```
$ cd mapasculturais-app
$ ionic state reset
$ bower install
```

* Fazer o setup SASS
```
$ ionic setup sass
```

* Rodar
```
$ ionic serve
```

* Para rodar no navegador(chrominum) desabilitando a verfificação de cross-origin:
```
chromium --disable-web-security
```
E abrir o URL [http://localhost:8100](http://localhost:8100)

# Editando
----------

Na raiz do projeto você terá o diretorio scss onde ficará seu sass. só editar!
O ionic serve já faz o watch dos arquivos, recompila na alteração e faz o 
livereolad

* Resources
  * http://ionicframework.com/docs/cli/sass.html
  * http://learn.ionicframework.com/formulas/working-with-sass/
  * http://ionicframework.com/docs/components

# Rodando no celular Android ou Emulador

Para isso, você precisará ter a SDK Android instalada

* Instala o phonegap
```
$ npm install phonegap
```

* Adiciona a plataforma android ao projeto (aqui, se a SDK não estiver
instalada já haverá falha)
```
$ ionic platform add android
```

* Aqui, precisamos ter um dispositivo plugado ao computador aceitando 
instalação de fontes desconhecidas e com o modo desenvolvedor ativado.
```
$ ionic run android
```

* Para emular, é necessário que se crie um disposivo usando o Android SDK Manager
```
$ android
```

* Uma vez criado o dispositivo
```
$ ionic emulate android
```

