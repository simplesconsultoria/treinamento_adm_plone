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

Acessar a linha de comando e se logar como 

A partir da linha de comando, instalar os pacotes necessários ao treinamento::

	yum install -y autoconf automake curl-devel expat-devel gcc gcc-c++ gettext-devel groff libtool libxslt ncurses-devel openssl-devel pcre-devel pkgconfig python-devel python-setuptools subversion subversion-devel zlib-devel openldap-devel compat-openldap cyrus-sasl-lib git

