=========================
Buildout do Treinamento
=========================

Preparação do ambiente
=========================

Vamos instalar os pacotes necessários para a compilação do ambiente modelo de um portal Plone.

Com base na máquina virtual distribuída temos:

	* **usuário**: treinamento
	* **senha**: treinamento

.. note:: A senha do usuário root é a mesma.

CentOS
--------

Acessar a linha de comando e se logar como **root**::

	su  -


Instalar os pacotes necessários ao treinamento::

	yum install -y autoconf automake curl-devel expat-devel gcc gcc-c++ gettext-devel groff libtool libxslt ncurses-devel openssl-devel pcre-devel pkgconfig python-devel python-setuptools subversion subversion-devel zlib-devel openldap-devel compat-openldap cyrus-sasl-lib git

Instalação do Python
======================

Ainda como usuário root, garantir que temos a última versão do setuptools do python instalado::

	cd /usr/local
	easy_install -U setuptools

Vamos então clonar o repositório contendo o buildout de versões de Python::

	git clone https://github.com/collective/buildout.python.git python

E executá-lo::

	cd /usr/local/python
    python bootstrap.py
    ./bin/buildout

