![](https://img.shields.io/github/license/ajunior/brmodelo-installer.svg)
![](https://img.shields.io/badge/platform-ubuntu%2018.04+%20|%20windows%207%20|%20windows%2010%20|%20macos%20x-blue.svg)

# brModelo Installer
Instalador para o [brModelo](https://github.com/chcandido/brmodelo), desenvolvido com o [Qt Installer Framework](https://wiki.qt.io/Qt-Installer-Framework). O instalador foi devidamente testado nas seguintes palataformas: ```Windows 10```, ```Ubuntu 18.04``` e ```macOS X (Mojave)```. 

> O brModelo é uma ferramenta *open source* de [modelagem ER](https://pt.wikipedia.org/wiki/Modelo_entidade_relacionamento), desenvolvida por [Carlos Henrique Cândido](https://github.com/chcandido), especialmente difundida no meio acadêmico nas disciplinas de Banco de Dados.

## Ajuda do brModelo
O Arquivo de ajuda da ferramenta é instalado automaticamente durante o processo de instalação.

## Java
O brModelo é desenvolvido em [Java](http://www.java.com) 8, logo é necessário a instalação do Java Runtime Enviroment (JRE) 1.8 para execução da aplicação. A instalação do Java pode ser feita direto do instalador do brModelo.

# Qt Installer Framework
O instalador foi desenvolvido usando a versão [3.0.6](https://download.qt.io/official_releases/qt-installer-framework/3.0.6/) do Qt Installer Framework.

# Workflow do Instalador
Este instalador segue um fluxo simples de telas, que permitem a escolha do diretório onde a aplicação será instalada, o nome do grupo no menu iniciar (somente para Windows), aceitação da licença da aplicação e a seleção e instalação dos componentes da aplicação (incluindo JRE 1.8 - opcional), conforme ilustração abaixo:

![](http://doc.qt.io/qtinstallerframework/images/ifw-user-flow-installing.png)

## Estrutura de diretórios e arquivos

    .
    ├── Config                        # Test files (alternatively `spec` or `tests`)
    │   ├── config.xml                # Load and stress tests
    └── packages
        ├── br.com.brmodelo           # Load and stress tests
            ├── data                  # Load and stress tests
                ├── brmodelo.7z       # Load and stress tests
            ├── meta                  # Load and stress tests
                ├── package.xml       # Load and stress tests
        ├── com.java                  # Load and stress tests
            ├── data                  # Load and stress tests
                ├── java.7z           # Load and stress tests
            ├── meta                  # Load and stress tests
                ├── package.xml       # Load and stress tests

**OBS:** Arquivos não citados acima não são utilizados para confecção do instalador.

# Download (Executável)

| Arquivo | Plataforma | Release |
| :--- | :--- | :--- |
| [brmodelo-320-inst.exe]() | Windows 10 | 20/01/2019 |
| [brmodelo-320-inst.bin]() | GNU/Linux | 20/01/2019 |
| [brmodelo-320-inst.dmg]() | macOS X | 20/01/2019 |

# Contribuições
A confecção deste instalador é uma tarefa bem simples, mas toda contribuição é válida. Bugs devem ser informados via [*issue*](https://github.com/ajunior/brmodelo-installer/issues), enquanto contribuições de código devem ser feitas via **_Pull Request_**.

# Autoria
Este instalador foi desenvolvido por Adjamilton Junior como parte integrande do projeto brModelo e licenciado pela [GNU General Public License v3.0](LICENSE).
> O Qt Installer Framework é de autoria da Qt Foundation e licenciado sob a GNU General Public License v3.0. O brModelo é de autoria de Carlos Henrique Cândido e licenciado sob a GNU General Public License v3.0. Java é marca registrada da Oracle Corporation.