# Bota Pressão
É um Plugin para o gerenciamento do wordpress que permite botar pressão nos politicos ;)

# Inserindo novos campos input, select e textarea

Atualmente podemos inserir 3 tipos de campos rapidamente usando a função get_metas em deputados.php:

```
function get_metas()´
{
  return array(
    array ( 
        'label' => 'Partido', 
        'slug'=>'deputado_partido' ,
        'info' => 'Nenhum Partido Informado' , 
        'html' => array ('
                        tag'=> 'input', 
                        'type' => 'text' 
                        )
        ),
    array ( 
        'label' => 'Proposta de Campanha', 
        'slug'=>'deputado_prooposta' ,
        'info' => 'Nenhum Proposta Encontrada', 
        'html' => array (
                        'tag'=> 'textarea', 
                        'rows' => 4 , 
                        'cols' => 50 
                        ) 
        ),
        array ( 
        'label' => 'Partidos', 
        'slug'=>'deputado_partidos' ,
        'info' => 'Nenhum Partido Encontrado', 
        'html' => array (
                        'tag'=> 'select', 
                        'options' => array (
                           array ( 'value' => 'PMDB' , 'content' => 'PARTIDO DO MOVIMENTO DEMOCRÁTICO BRASILEIRO' ) ,
                           array ( 'value' => 'PTB' , 'content' => 'PARTIDO TRABALHISTA BRASILEIRO' ) 
                          )
                        ) 
        ),
  ); 
}
```
