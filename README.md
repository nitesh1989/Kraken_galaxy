How to test Kraken in your local galaxy instance:

In your galaxy home directory config/tool_conf.xml file, change  

```
 <section name="Kraken-test" id="kraken">
    <tool file="/full-path/Kraken_galaxy/kraken.xml" />
 </section>
 ```

In the config/tool_data_table_conf.xml, add this:

```
<table name="krakendb" comment_char="#">
    <columns>value ,dbkey, display_name, file_path</columns>
    <file path="/Users/nturaga/Documents/Kraken_galaxy/tool-data/kraken_database.loc" />
</table>
```