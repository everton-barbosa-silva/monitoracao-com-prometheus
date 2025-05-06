Laboratório de Monitoramento com Prometheus, Grafana e NGINX

Este projeto configura um ambiente local de monitoramento com Prometheus, Grafana e NGINX como proxy reverso, utilizando domínios locais como `grafana.intranet` e `prometheus.intranet`.

---

Requisitos

- Docker
- Docker Compose
- Sistema Linux com acesso ao `/etc/hosts`
- Navegador web moderno

---

Estrutura do Projeto

monitoring-lab/
├── docker-compose.yml
├── nginx/
│ └── default.conf
├── prometheus.yml
└── README.md



---

 Configuração Local

Adicione os domínios locais no `/etc/hosts`

Execute:

```bash
sudo vim /etc/hosts

Adicione as seguintes linhas:


127.0.0.1 grafana.intranet
127.0.0.1 prometheus.intranet



docker-compose up -d
