---
weight: 20
title: TableSnapshotResponse
aliases:
  - /reference/eosio/types/tablesnapshotresponse/

---

## Type `TableSnapshotResponse`

#### Properties

{{< method-list-item name="type" type="String" required="true" >}}
   The `table_snapshot` string
{{< /method-list-item >}}

{{< method-list-item name="data" type="[TableRows](/eosio/public-apis/reference/types/tablerows)" required="true" >}}
   Rows for the corresponding `get_table_rows` request. The `TableRows` object will not contain `account` nor `scope` in this case.
{{< /method-list-item >}}

## Example Payload

{{< highlight json >}}
{"type": "table_snapshot",
 "req_id": "your-request-id",
 "data": {
  "rows": [
   {
    ...
   }]
}}
{{< /highlight >}}
