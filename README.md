ansible-postfix-to-mandrill role
================================

This role installs Postfix as a [Mandrill](https://mandrillapp.com/) relayer

# Variables

- `postfix_to_mandrill_username`: Mandrill username (usually and email, default: false, mandatory)
- `postfix_to_mandrill_password`: Mandrill password (i.e. API Key, default: false, mandatory)
- `postfix_to_mandrill_use_submission`: Use submission port (default: true)
- `postfix_to_mandrill_relayhost`: Mandril SMTP relay (default: smtp.mandrillapp.com, probably always good, defined in `vars/main.yml`)

# Misc 

- No dependencies
- Installs mailutils


Michel Blanc <mb@mbnet.fr>
