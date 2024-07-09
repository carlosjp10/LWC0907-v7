<apex:page>
    <html>
    <style>
        a {
            color:blue;
        }
    </style>

    <script src="https://leonardi--dev.sandbox.my.salesforce-sites.com/lightning/lightning.out.js"></script>
    <div data-lightning-out="true"></div>

    <script>
        const appName = 'c:testeGlobalApp';
        const componentName = 'c:gerenciarItensCotacao';
        const lightningEndpoint = 'https://leonardi--dev.sandbox.my.salesforce-sites.com';
        const targetElement = document.querySelector("[data-lightning-out]");
        const componentAttributes = {

        };

        $Lightning.use(
            appName,
            function(){
                $Lightning.createComponent(
                    componentName,
                    componentAttributes,
                    targetElement,
                    function(cmp){
                        console.log('@cac funcionando');
                    }
                );
            },
            lightningEndpoint
        );
    </script>
</html>
</apex:page>
