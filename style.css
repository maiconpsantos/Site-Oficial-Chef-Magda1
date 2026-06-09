const menuToggle = document.getElementById("menuToggle");
const menu = document.getElementById("menu");

menuToggle.addEventListener("click", () => {
  menu.classList.toggle("open");
});

document.querySelectorAll(".service-body a[data-servico]").forEach((link) => {
  link.addEventListener("click", () => {
    const servico = link.getAttribute("data-servico");
    setTimeout(() => {
      document.getElementById("servico").value = servico;
    }, 100);
  });
});

document.getElementById("formOrcamento").addEventListener("submit", function (event) {
  event.preventDefault();

  const telefoneDestino = "5541997523844";

  const nome = document.getElementById("nome").value.trim();
  const telefone = document.getElementById("telefone").value.trim();
  const servico = document.getElementById("servico").value;
  const data = document.getElementById("data").value;
  const pessoas = document.getElementById("pessoas").value.trim();
  const observacoes = document.getElementById("observacoes").value.trim();

  const mensagem = `Olá, Chef Magda! Gostaria de solicitar um orçamento.

Nome: ${nome}
WhatsApp para contato: ${telefone}
Serviço desejado: ${servico}
Data: ${data || "Não informada"}
Quantidade de pessoas: ${pessoas || "Não informada"}
Observações: ${observacoes || "Nenhuma observação."}`;

  const url = `https://wa.me/${telefoneDestino}?text=${encodeURIComponent(mensagem)}`;
  window.open(url, "_blank");
});
