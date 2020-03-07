Ansible Role: wkhtmltopdf
=========

本 Role 用于在PHP运行环境下安装 [wkhtmltopdf](https://wkhtmltopdf.org/)。

## Requirements

运行本 Role，请确认符合如下的必要条件：

| **Items**      | **Details** |
| ------------------| ------------------|
| Operating system | CentOS7.x Ubuntu18.04 AmazonLinux |
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


