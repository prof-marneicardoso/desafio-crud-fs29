# Buenas Imóveis — Sistema de Imobiliária com CRUD

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![LocalStorage](https://img.shields.io/badge/LocalStorage-333?style=for-the-badge&logo=databricks&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222?style=for-the-badge&logo=githubpages&logoColor=white)

## Projeto CRUD como Desafio para fixar o conhecimento em JS, DOM, Local Storage e JSON.

> **Projeto didático** simulando um cenário profissional real com briefing de cliente, quadro de tasks e entrega com deploy. Vamos simular o pedido de um cliente para a minha empresa de desenvolvimento, com os estudantes sendo os colaboradores. Como Dev, precisam ler o enunciado e seguir os requisitos solicitados.

## 📌 Sobre o Projeto

A **Buenas Imóveis** é um sistema Web de cadastro e gerenciamento de imóveis, desenvolvido como MVP (Produto Mínimo Viável) para a cliente fictícia **Sra. Helen Bueno**, proprietária de uma imobiliária de pequeno porte em Porto Alegre/RS.

O sistema funciona 100% no navegador, utilizando **localStorage** para persistência dos dados e **manipulação de DOM** para renderização dinâmica da interface. Os dados são estruturados em **JSON**.

### Funcionalidades

- **CRUD completo**: Cadastrar, Listar, Editar e Excluir imóveis
- **Persistência**: Dados salvos no `localStorage` (não perde ao fechar o navegador)
- **Tags visuais**: Distinção de **Venda** (verde) e **Aluguel** (azul) com cores diferentes
- **Tipos de imóvel**: Casa, Apartamento, Terreno e Sala
- **Finalidade**: Residencial ou Comercial
- **Status**: Imóveis ativos (visíveis) ou inativos (rascunho)
- **Múltiplas fotos**: Suporte a várias URLs de fotos por imóvel
- **Google Maps**: Link de embed para localização do imóvel
- **Valores formatados**: Exibição em R$ (moeda brasileira)
- **Página de detalhe**: Visualização completa do imóvel em nova aba
- **Modal de edição**: Edição via `<dialog>` nativo do HTML
- **Busca e filtros**: Por título, localização, tipo, venda/aluguel e faixa de valor
- **Responsivo**: Funciona em desktop, tablet e celular

---

## 🎯 Cenário Profissional

Este projeto simula uma demanda real de desenvolvimento. O aluno assume o papel de **desenvolvedor(a) junior** e recebe o projeto organizado em **Tasks**, como acontece em empresas de tecnologia.

---

## 📋 Briefing da Cliente

"Marnei, tô precisando de um site urgente! Hoje controlo tudo numa planilha e tô perdendo negócio. Preciso cadastrar meus imóveis pelo celular ou computador, com fotos, preço, localização, tudo. Quero que o pessoal que entra no site veja os imóveis bem bonitos com foto, e consiga ver se é pra VENDA ou ALUGUEL. Os preços têm que aparecer formatados bonitinho, tipo R$ 450.000,00. Preciso poder corrigir erros de digitação (editar), excluir imóveis vendidos, e o mais importante: NÃO POSSO PERDER OS DADOS quando fechar o navegador! Ah, e preciso separar se é casa, apartamento, terreno ou sala, e se é residencial ou comercial. Tem imóvel que eu quero deixar cadastrado mas não aparecer no site ainda, tipo um rascunho. E quero um link do Google Maps em cada imóvel."

### Mensagem para a equipe:

"A Dona Helen Bueno precisa desse MVP rodando o mais rápido possível. Nesta primeira sprint, o sistema vai funcionar 100% no navegador usando localStorage. Quando ela aprovar o visual e as funcionalidades, a gente conecta num Back-End de verdade. O site vai ter duas partes: uma página Home pública onde qualquer pessoa vê os imóveis ativos, e ao clicar em um imóvel, abre uma página de detalhe com todas as informações. O cadastro, edição e exclusão ficam na própria Home por enquanto (na sprint 2 a gente separa num painel admin com login). Organizei o desenvolvimento em Tasks. Sigam a ordem, façam commits organizados e caprichem, a cliente vai ver o resultado. Boora!"

### O que a cliente precisa (URGENTE):

```
✅ Cadastrar imóveis pelo celular/computador
✅ Ver todos os imóveis em cards bonitos (com foto!)
✅ Distinguir VENDA de ALUGUEL na hora (cores diferentes?)
✅ Preços formatados (R$ 450.000,00)
✅ Poder corrigir erros de digitação
✅ Excluir imóveis vendidos/alugados
✅ NÃO PERDER DADOS quando fechar o navegador!
```

### Dados levantados na reunião

**Nome da marca**: Buenas Imóveis

**Cores da marca**: Roxo (#6c5fff) e cinza escuro (#232323)

**Fonte:** Poppins (Google Fonts)

Estrutura de dados de cada imóvel:

```json
{
    "id": 1,
    "titulo": "Casa com 3 quartos no Menino Deus",
    "descricao": "Ampla casa com garagem para 2 carros, quintal com churrasqueira e área de lazer.",
    "valor": 450000,
    "area": 180,
    "quartos": 3,
    "tipo": "casa",
    "localizacao": "Menino Deus - Porto Alegre/RS",
    "mapa": "https://www.google.com/maps/embed?pb=...",
    "venda_aluguel": "venda",
    "finalidade": "residencial",
    "fotos": [
        "https://exemplo.com/foto1.jpg",
        "https://exemplo.com/foto2.jpg"
    ],
    "status": true,
    "created_at": "2026-03-08T14:30:00.000Z"
}
```


