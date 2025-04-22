Linux Nftables
=========

Un role pour configurer nftables

Requirements
------------

- Le paquet sudo

Role Variables
--------------

| Nom de la variable | Obligatoire | Type       | Valeur par defaut | Description                                        |
|--------------------|-------------|------------|-------------------|----------------------------------------------------|
| lx_nftables_input  | false       | list[dict] |                   | Une list de règles pour les paquets entrants       |
| lx_nftables_output | false       | list[dict] |                   | Une list de règles pour les paquets sortants       |
| lx_nftables_forwrd | false       | list[dict] |                   | Une list de règles pour les paquets qui transitent |


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
