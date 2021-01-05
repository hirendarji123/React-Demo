import React, { useState } from 'react';
import MaterialTable from 'material-table';

import Navbar from './Navbar'

const MaterialUuTable = () => {
  const { useState } = React;

  const [data, setData] = useState([
    { name: 'Arpit', surname: 'xyz',  birthCity: 40 },
    { name: 'Hiren', surname: 'Baran',  birthCity: 23 },
    { name: 'Mehmet', surname: 'Baran',  birthCity: 50},
    { name: 'Priti', surname: 'Baran',  birthCity: 34 },
    { name: 'Viren', surname: 'Baran',  birthCity: 25 },
    { name: 'Zara', surname: 'Baran',  birthCity: 43 },
  ]);
  const [columns, setColumns] = useState([

    { title: 'Name', field: 'name', editable: 'onUpdate', type: 'stirng', grouping: false, validate: rowData => rowData.name === '' ? { isValid: false, helperText: 'Name cannot be empty' } : true },
    { title: 'Surname', field: 'surname', editable: 'never' },
    {
      title: 'Birth Place',
      field: 'birthCity',
      type:'string'
    }
  ]);






  return (
    <>
      <Navbar />
      <h1 style={{ textAlign: "center", color: "white",backgroundColor:"gray"}}>UI Material Table</h1>
      <MaterialTable title="Table"
        data={data}
        columns={columns}
        options={{
          filtering: true,
          exportButton: true
        }}

      />


    </>
  )
}
export default MaterialUuTable;