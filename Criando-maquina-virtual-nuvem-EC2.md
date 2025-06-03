# AWS: Criando uma Máquina Virtual em Nuvem (EC2)

## O que é EC2?

O **Amazon EC2 (Elastic Compute Cloud)** é como alugar um computador na nuvem da AWS. Você pode escolher o tamanho, o sistema operacional e instalar o que quiser, pagando só pelo tempo de uso.

---

## Por que usar EC2?

- **Escalável:** Crie 1 ou 1000 máquinas em minutos.
- **Flexível:** Escolha Windows, Linux, memória, CPU, etc.
- **Econômico:** Pague só pelo que usar.

---

## Exemplo Lúdico

Imagine que você vai dar uma festa (seu site/app). Em vez de comprar um salão (servidor físico), você aluga um espaço na hora (EC2). Se mais convidados chegarem, você aluga mais espaço rapidinho!

---

## Exemplo Real: Criando uma EC2 Linux

1. **Acesse o Console AWS:**  
    https://console.aws.amazon.com/ec2/

2. **Clique em "Executar Instância".**

3. **Escolha uma AMI:**  
    Exemplo: Ubuntu Server 22.04 LTS.

4. **Escolha o Tipo de Instância:**  
    Exemplo: t2.micro (grátis no Free Tier).

5. **Configurar Chave SSH:**  
    Crie ou use uma chave para acessar via terminal.

6. **Configurar Segurança:**  
    Libere a porta 22 (SSH) para acessar remotamente.

7. **Lançar Instância!**

---

## Acessando sua EC2

No terminal, digite:

```bash
ssh -i "sua-chave.pem" ubuntu@<IP-da-instancia>
```

---

## Pronto!

Você agora tem um servidor Linux na nuvem, pronto para instalar sites, bancos de dados ou o que quiser!
