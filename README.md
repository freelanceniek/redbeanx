# redbeanx

Redbean (ORM?) with support for custom id fields and fkey fields to support existing databases

Sofar the rb.php version 4 is modified to rbx.php to support custom id fields.

You have to tell redbean what the name of the id field is (if not "id")

R::getRedBean()->idFieldMap= array('adres'=>'id_adres','contact'=>'contact_id'); // setup after Redbean database was setup



Future improvements: support custom Foreign keys.

R::getRedBean()->fkeyFieldMap=array('source_tablename'=>['dest_tablename'=>'fkey_fieldname']);
