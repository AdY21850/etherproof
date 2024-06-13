pragma solidity 0.8.18;

contract MyToken {
    string public name;      
    string public symbol;     
    uint256 public totalSupply;  
    
    mapping(address => uint256) public balances;

    constructor(string memory _name, string memory _symbol, uint256 _totalSupply) {
        name = _name;
        symbol = _symbol;
        totalSupply = _totalSupply;
        balances[msg.sender] = _totalSupply; 
    }

    
    function mint(address account, uint256 amount) public {
        totalSupply += amount;
        balances[account] += amount;
    }

    
    function burn(address account, uint256 amount) public {
        require(balances[account] >= amount, "Insufficient balance");
        totalSupply -= amount;
        balances[account] -= amount;
    }
}
