describe('Teste de requisição GET para API do Trello', () => {
     const key = '592f11060f95a3d3d46a987a'
  it('Deve obter o conteúdo do campo "name" da estrutura "list" e validar o status code da resposta', () => {
   
    // Envia uma solicitação GET para a API do Trello
    cy.request({
      method: 'GET',
      url: `https://api.trello.com/1/actions/${key}`, headers: { token }
      
    }).then((response) => {
      // Verifica se a solicitação foi bem-sucedida (código de status 200)
      expect(response.status).to.eq(200);

      // Obtém o conteúdo JSON da resposta
      

      // Exibe o conteúdo do campo "name" da estrutura "list"
      const Name = response.body;
      cy.log("Nome da lista:", Name);
    });
  });
});
