Linux Nftables
=========

Un role pour configurer nftables

Requirements
------------

- Le paquet sudo

Role Variables
--------------

| Nom de la variable            | Obligatoire | Type       | Valeur par defaut | Description                                           |
|-------------------------------|-------------|------------|-------------------|-------------------------------------------------------|
| lx_nftalbes_established       | false       | bool       | True              | Autoriser les réponses à des connexions déjà initiées |
| lx_nftables_input_log_prefix  | false       | str        | Denied input:     | Prefix de log pour les paquets entrants               |
| lx_nftables_input_policy      | false       | str        | drop              | Règle pour les paquets entrants                       |
| lx_nftables_input             | false       | list[dict] |                   | Une liste de règles pour les paquets entrants         |
| lx_nftables_output_log_prefix | false       | str        | Denied output:    | Prefix de log pour les paquets sortant                |
| lx_nftables_output_policy     | false       | str        | drop              | Règle pour les paquets sortants                       |
| lx_nftables_output            | false       | list[dict] |                   | Une liste de règles pour les paquets sortants         |
| lx_nftables_input_log_prefix  | false       | str        | Denied forward:   | Prefix de log pour les paquets en transitent          |
| lx_nftables_forward_policy    | false       | str        | drop              | Règle pour les paquets en transitent                  |
| lx_nftables_forwrd            | false       | list[dict] |                   | Une liste de règles pour les paquets qui transitent   |


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
