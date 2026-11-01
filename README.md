# 💅 Agenda Vívian Martins

Site de agendamento online para a manicure **Vívian Martins** (Londrina/PR).

🔗 **Site no ar:** [vivianmartins.netlify.app](https://vivianmartins.netlify.app)

## Como funciona

1. A cliente escolhe um ou mais serviços (com preço e duração)
2. Escolhe o dia (terça a sábado) e o horário
3. Preenche nome e WhatsApp
4. O site monta a mensagem do pedido e envia direto pro WhatsApp da profissional

## Funcionalidades

- Lista de serviços com soma automática do total e da duração
- Calendário dos próximos 14 dias de atendimento
- Horários que já passaram ficam bloqueados
- Horários que estouram o fim do expediente ficam bloqueados conforme a duração do serviço
- Mensagem pronta pro WhatsApp (botão de enviar e de copiar)
- Layout responsivo (celular e PC) com tema claro e escuro automático

## Tecnologias

- HTML, CSS e JavaScript puro (sem framework)
- Google Fonts (Bodoni Moda, Great Vibes, Nunito Sans)
- Hospedagem: Netlify

## Como configurar

Tudo fica no começo do `<script>` do `index.html`:

```js
const WHATSAPP = "5543999999999";     // número com DDI + DDD
const DIAS_ATENDE = [2, 3, 4, 5, 6];  // 0 = domingo ... 6 = sábado
const HORARIOS = ["08:00", "09:00", ...];
const FECHA = "19:00";                // fim do expediente
const SERVICOS = [ { nome: "Alongamento", preco: 150, min: 150 }, ... ];
```

## Próximos passos

- [ ] Tela inicial com galeria de fotos dos trabalhos
- [ ] Pular horário de almoço no cálculo
- [ ] Salvar agendamentos no Firebase e bloquear horários ocupados
- [ ] Painel com login pra profissional ver e confirmar a agenda

---

Feito por **Claudio Silva** — estudante de Técnico em Desenvolvimento de Sistemas (CEEP Londrina).