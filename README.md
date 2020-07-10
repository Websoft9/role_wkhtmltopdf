Ansible Role: wkhtmltopdf
=========

This rols is install the [wkhtmltopdf](https://wkhtmltopdf.org/) and some Fonts

## Requirements

运行本 Role，请确认符合如下的必要条件：

| **Items**      | **Details** |
| ------------------| ------------------|
| Operating system | CentOS7.x Ubuntu16.04,18.04 AmazonLinux |
| Python 版本 | Python2  |
| Python 组件 |    |
| Runtime |  |


## Related roles

本 Role 在运行时需要确保已经运行：common。以下为例：

```
roles:
    - {role: role_common, tags: "role_common"}
    - {role: role_wkhtmltopdf, tags: "role_wkhtmltopdf"}
```


## Variables

暂无

## Example

```
- name: wkhtmltopdf
  hosts: all
  become: yes
  become_method: sudo 
  vars_files:
    - vars/main.yml 

  roles:
    - { role: role_common }
    - { role: role_wkhtmltopdf }
    ...
```

## FAQ


