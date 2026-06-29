Wanbo RC v0.6

Correções desta versão:
1. Inversão visual dos ícones:
   - botão selecionado fica escuro;
   - botões não selecionados ficam claros.
2. Ícone do app corrigido:
   - wanbo_rc.png é 10x10, 1-bit, sem transparência.
3. application.fam mantém:
   - name="Wanbo RC"
   - fap_icon="wanbo_rc.png"

Atenção sobre a mensagem:
"App Too Old. APP:86 < FW:87"

Isso NÃO é corrigido no código do app. É a versão do SDK usada pelo uFBT.
Para corrigir, atualize o SDK do uFBT no ambiente onde você compila:

    ufbt update
    ufbt -c
    ufbt

Se ainda aparecer APP:86 < FW:87, use:

    ufbt update --channel=dev
    ufbt -c
    ufbt

Se o app continuar aparecendo como "wanbo_rc" na lista, apague o .fap antigo do Flipper e copie o novo.
Se o menu do seu firmware exibir o nome pelo arquivo, renomeie o arquivo compilado de:

    wanbo_rc.fap

para:

    Wanbo RC.fap

e copie para:

    SD Card/apps/Infrared/
