# Context Menu For Windows11

Demos  For Add Context Menu

* 7zContextMenu : add [7z Extract Here] Menu


```xml

    <desktop4:Extension Category="windows.fileExplorerContextMenus">
          <desktop4:FileExplorerContextMenus>
            <desktop5:ItemType Type="*"  >
              <desktop5:Verb Id="Command1" Clsid="46F650E5-9959-48D6-AC13-A9637C5B3787" />
            </desktop5:ItemType>
          </desktop4:FileExplorerContextMenus>
        </desktop4:Extension>
        <com:Extension Category="windows.comServer">
          <com:ComServer>
            <com:SurrogateServer  DisplayName="Context menu verb handler">
              <com:Class Id="46F650E5-9959-48D6-AC13-A9637C5B3787" Path="7zContextMenu2\7zContextMenuHost.dll" ThreadingModel="STA"/>
            </com:SurrogateServer>
          </com:ComServer>
        </com:Extension>

```


more  

https://docs.microsoft.com/en-us/windows/apps/desktop/modernize/desktop-to-uwp-extensions#context-menu

https://github.com/MicrosoftDocs/winrt-related/blob/docs/winrt-related-src/schemas/appxpackage/uapmanifestschema/element-desktop5-itemtype.md

https://github.com/microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/shell/appshellintegration/ExplorerCommandVerb

https://github.com/microsoft/AppModelSamples/tree/0f88fe0a8bbb90051f6c126741b881288bb5cabb/Samples/SparsePackages/PhotoStoreContextMenu

https://github.com/microsoft/terminal/blob/c90de692509b074bfde191910d67154cfe389911/src/cascadia/CascadiaPackage/Package.appxmanifest

https://github.com/microsoft/terminal/tree/fb597ed304ec6eef245405c9652e9b8a029b821f/src/cascadia/ShellExtension

https://github.com/MicrosoftDocs/windows-uwp/blob/docs/hub/apps/desktop/modernize/integrate-packaged-app-with-file-explorer.md