# Online Shop

## 1. **Stripe CLI**

```bash
stripe listen --forward-to 127.0.0.1:8000/payment/webhook/
```

## 2. **Celery**

```bash
celery -A myshop worker -l info
celery -A myshop beat -l info
celery -A myshop flower -l info
```

## 3. **RabbitMQ with Docker**

```bash
sudo docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13.1-management
```