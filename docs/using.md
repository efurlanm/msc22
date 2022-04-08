# Using de environment

A aplicação web JN é baseada em um framework cliente-servidor, que permite sua utilização em uma única ou em várias máquinas, e permitindo que o código seja executado em qualquer uma delas. Dessa forma, é possível trabalhar no laptop pessoal e ao mesmo tempo executar o código em uma máquina remota (por exemplo, SDumont). 

Ao usar o JL não é necessário usar o shell SSH CLI tradicional, e tudo pode ser feito usando a interface JN. Inclusive o JN pode ser executado em sistemas operacionais diferentes (Windows, Linux, MacOS), em máquinas locais e remotas, e a interface padrão no navegador web permanece a mesma para o usuário, independente de onde o servidor está rodando.

A ideia por trás do desenvolvimento usando JN no SDumont, eu acho, é que a maior parte do trabalho de desenvolvimento é feito no laptop pessoal e, em seguida, o SDdumont é usado para compilar o código final, executá-lo e obter os resultados, tudo usando o ambiente JN. Apenas o trabalho que é computacionalmente intensivo e requer desempenho é feito no SDumont. A análise dos dados obtidos, geração de gráficos e documentação também é feita no laptop pessoal, utilizando o mesmo ambiente JN. O que muda é que uma máquina estará em uma aba do navegador web, e a outra máquina estará em outra aba do navegador web. Máquinas diferentes estarão em abas diferentes do navegador da web. 

É importante observar que apesar de utilizar o navegador web, não é necessário estar conectado à internet ao executar o JN localmente. Acho que talvez a melhor maneira de usar o JN seja executar dois Notebook Servers (NS), um rodando permanentemente no laptop e o outro rodando eventualmente no SDumont apenas para enviar trabalhos e depois novamente para obter os resultados. As tarefas que não são computacionalmente intensivas são executadas no laptop (máquina local). O JN utiliza um arquivo no formato texto com extensão .ipynb que pode ser configurado para ser salvo automaticamente. Este arquivo pode ser copiado para a máquina local, visualizado e editado, tanto no JN quanto em um editor de texto comum. Desta forma não é necessário estar permanentemente conectado ao SDumont. A cópia de arquivos entre máquinas também pode ser feita via GUI, usando, por exemplo, o gerenciador de arquivos Dolphin e o protocolo fish. Outra maneira, talvez ainda melhor, dependendo da situação, pode ser usar sshfs para montar um sistema de arquivos remoto e usar JN para fazer a cópia, embora em alguns casos isso possa causar alguma confusão (este caso será discutido mais adiante).




An important detail about using CE together with JL is that when starting the JL server, the CE must already be configured, and the JL must be started in the working directory so that it becomes the JL root directory. So let's suppose we have three CEs, one environment for each different job we're doing, and the names are, for example, env01, env02, and env03. Let's also assume that we have three working directories, named work01, work02, and work03. To activate them, we would do:

source /scratch/app/anaconda3/2020.11/etc/profile.d/conda.sh
cd work01
conda activate --stack /scratch/ampemi/<username>/env01




ST
 Ao trabalhar com várias máquinas (por exemplo, um PC, um laptop e o SDdumont), também é possível sincronizar automaticamente o mesmo diretório entre máquinas, de forma que o arquivo em que estamos trabalhando seja sempre o mais atual, e todos as alterações feitas nele são atualizadas automaticamente nas outras máquinas, sem que precisemos nos preocupar com isso. Além destes, a ferramenta também possui vários outros recursos úteis.
