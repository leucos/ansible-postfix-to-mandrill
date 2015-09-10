ansible-postfix-to-mandrill role
================================

This role installs Postfix as a [Mandrill](https://mandrillapp.com/) relayer

# Variables

- `postfix_to_mandrill_username`: Mandrill username (usually and email, default: false, mandatory)
- `postfix_to_mandrill_password`: Mandrill password (i.e. API Key, default: false, mandatory)
- `postfix_to_mandrill_use_submission`: Use submission port (default: true)
- `postfix_to_mandrill_relayhost`: Mandril SMTP relay (default: smtp.mandrillapp.com, probably always good, defined in `vars/main.yml`)
- `postfix_to_mandrill_subaccount`: sub-account header to use if needed (default: none); see https://mandrill.zendesk.com/hc/en-us/articles/205583317-How-do-I-create-a-subaccount-


postfix_to_mandrill_default_sender: "root@{{ inventory_hostname }}"


# Misc 

- No dependencies
- Installs mailutils

# Caveats

This will override any postfix config you might have, so you need to adapt this
role to fit your needs if they are not covered.

PRs welcomed !

Michel Blanc <mb@mbnet.fr>
