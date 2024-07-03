import React, { useState } from 'react';

function Clicar() {
    const [click, setClick] = useState(0);

    const qtdClicks = () => {
        setClick(click + 1);
    };

    return (
        <div>
            <p>Numero de clicks: {click}</p>
            <button onClick={qtdClicks}>Click</button>
        </div>
    );
}

export default Clicar;
