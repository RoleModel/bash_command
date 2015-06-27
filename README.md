# bash_command

Will execute the passed `command` in the passed `dir`. Useful for doing things like bundle install and rake db:migrate via a role.

```yml
- hosts: defaults
  roles:
    - { role: bash_command, dir: '/var/www/my_app', command: 'bundle install' }
    - { role: bash_command, dir: '/var/www/my_app', command: 'bundle exec rake db:migrate' }
```

## License

* MIT
