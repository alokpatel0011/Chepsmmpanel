    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    
    body {
        background-color: var(--light);
        color: var(--dark);
    }
    
    header {
        background-color: var(--primary);
        color: white;
        padding: 1rem 2rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
        box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    
    .logo {
        font-size: 1.8rem;
        font-weight: bold;
    }
    
    nav ul {
        display: flex;
        list-style: none;
    }
    
    nav ul li {
        margin-left: 1.5rem;
    }
    
    nav ul li a {
        color: white;
        text-decoration: none;
        font-weight: 500;
        transition: all 0.3s ease;
    }
    
    nav ul li a:hover {
        color: var(--secondary);
    }
    
    .cart-icon {
        position: relative;
        cursor: pointer;
    }
    
    .cart-count {
        position: absolute;
        top: -10px;
        right: -10px;
        background-color: var(--danger);
        color: white;
        border-radius: 50%;
        width: 20px;
        height: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 0.8rem;
    }
    
    .hero {
        background: linear-gradient(135deg, var(--primary), var(--secondary));
        color: white;
        padding: 4rem 2rem;
        text-align: center;
    }
    
    .hero h1 {
        font-size: 2.5rem;
        margin-bottom: 1rem;
    }
    
    .hero p {
        font-size: 1.2rem;
        max-width: 800px;
        margin: 0 auto 2rem;
    }
    
    .search-bar {
        max-width: 600px;
        margin: 0 auto;
        display: flex;
    }
    
    .search-bar input {
        flex: 1;
        padding: 0.8rem 1rem;
        border: none;
        border-radius: 4px 0 0 4px;
        font-size: 1rem;
    }
    
    .search-bar button {
        background-color: var(--dark);
        color: white;
        border: none;
        padding: 0 1.5rem;
        border-radius: 0 4px 4px 0;
        cursor: pointer;
        transition: all 0.3s ease;
    }
    
    .search-bar button:hover {
        background-color: #1e272e;
    }
    
    .container {
        max-width: 1200px;
        margin: 2rem auto;
        padding: 0 1rem;
    }
    
    .section-title {
        font-size: 1.8rem;
        margin-bottom: 1.5rem;
        position: relative;
        padding-bottom: 0.5rem;
    }
    
    .section-title::after {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 60px;
        height: 3px;
        background-color: var(--primary);
    }
    
    .products {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
        gap: 1.5rem;
    }
    
    .product-card {
        background-color: white;
        border-radius: 8px;
        overflow: hidden;
        box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        transition: all 0.3s ease;
    }
    
    .product-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }
    
    .product-image {
        height: 180px;
        background-color: #eee;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 3rem;
        color: var(--dark);
    }
    
    .product-info {
        padding: 1.5rem;
    }
    
    .product-title {
        font-size: 1.2rem;
        margin-bottom: 0.5rem;
    }
    
    .product-description {
        color: #666;
        margin-bottom: 1rem;
        font-size: 0.9rem;
    }
    
    .product-price {
        font-size: 1.3rem;
        font-weight: bold;
        color: var(--primary);
        margin-bottom: 1rem;
    }
    
    .add-to-cart {
        width: 100%;
        padding: 0.7rem;
        background-color: var(--primary);
        color: white;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        transition: all 0.3s ease;
    }
    
    .add-to-cart:hover {
        background-color: #5649c0;
    }
    
    .categories {
        display: flex;
        flex-wrap: wrap;
        gap: 1rem;
        margin-bottom: 2rem;
    }
    
    .category {
        padding: 0.5rem 1rem;
        background-color: white;
        border-radius: 20px;
        cursor: pointer;
        transition: all 0.3s ease;
        box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    
    .category:hover, .category.active {
        background-color: var(--primary);
        color: white;
    }
    
    footer {
        background-color: var(--dark);
        color: white;
        padding: 3rem 2rem;
        margin-top: 3rem;
    }
    
    .footer-content {
        max-width: 1200px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 2rem;
    }
    
    .footer-column h3 {
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
        position: relative;
        padding-bottom: 0.5rem;
    }
    
    .footer-column h3::after {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 40px;
        height: 2px;
        background-color: var(--primary);
    }
    
    .footer-column ul {
        list-style: none;
    }
    
    .footer-column ul li {
        margin-bottom: 0.8rem;
    }
    
    .footer-column ul li a {
        color: #b2bec3;
        text-decoration: none;
        transition: all 0.3s ease;
    }
    
    .footer-column ul li a:hover {
        color: white;
    }
    
    .copyright {
        text-align: center;
        margin-top: 2rem;
        padding-top: 2rem;
        border-top: 1px solid rgba(255,255,255,0.1);
        color: #b2bec3;
    }
    
    /* Cart Modal */
    .modal {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0,0,0,0.5);
        z-index: 1000;
        justify-content: center;
        align-items: center;
    }
    
    .modal-content {
        background-color: white;
        width: 90%;
        max-width: 800px;
        max-height: 80vh;
        border-radius: 8px;
        overflow: hidden;
        display: flex;
        flex-direction: column;
    }
    
    .modal-header {
        padding: 1rem;
        background-color: var(--primary);
        color: white;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    
    .close-modal {
        font-size: 1.5rem;
        cursor: pointer;
    }
    
    .modal-body {
        padding: 1.

        <!DOCTYPE html>
