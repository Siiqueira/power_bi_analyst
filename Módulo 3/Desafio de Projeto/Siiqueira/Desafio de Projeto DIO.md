# 🚀  Desafio de Projeto DIO 

### Etapas de Processo

- Realizei a criação do banco de dados no MySQL Workbench, pois tive problema com o Azure e m minha conta.
- Criei o banco de dados chamado azure_company.
- Criei as tabelas employee, departament, dependent, project, dept_locations e works_on.
- Adcionei os dados puxando do Github do expert.
- Fiz a integeção do Power BI com o MySQL.
- Comecei a fazer as Transformações dos dados com o Power Query.
- Verifiquei os cabeçalhos, valores nulos, definindo monetário para coluna salary, verifiquei duplicidade.
- verifiquei colaboradores por gerente.
- verifiquei departamento sem gerente.
- separei a coluna Address.
- verificado quantas horas por projeto.
- Realizei a mesclagem de de consulta de employee e departament, usando a tabela employee como referência.
- realizei a junção de colaboradores por gerente. utilizei o próprio Power Query para fazer.
  realizei a mesclagem da tabela employee com ela mesmo usando as colunas Super_ssn e Ssn para realizar a junção depois desse processo eu realizei a mesclagem de coluna para juntar Fname e Lname;
  
#### Esse processo no MySQL seria esse processo:

  SELECT
    concat(g.Fname, ' ', g.Lname) AS Gerente,
    concat(e.Fname, ' ', e.Lname) AS Colaborador
    
FROM 
    employee e
LEFT JOIN 
    employee g ON e.Super_ssn = g.Ssn;
    

- Realizei a mesclagem dos nomes dos Departamentos e a localização para combinação departamento-local.
- nesse caso devemos fazer a mesclagem, por que com a mesclagem retornamos os valores relacionados. atribuir irá adicionar os dados duplicando outros dados e criando dados nulos. que seria um problema.
- criado o relátorio.



    
