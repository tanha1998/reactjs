Routes
> GET    /api/products
> GET    /api/products/:id
> POST   /api/products
> PUT    /api/products/:id
> DELETE /api/products/:id
Filter
gt = greater than, gte = greater than or equal.
lt = lesser than, lte = lesser than or equal.
> GET /api/products?price=15
> GET /api/products?price[gt]=15.99
> GET /api/products?price[gte]=15.99
> GET /api/products?price[lt]=15.99
> GET /api/products?price[lte]=15.99
> GET /api/products?title[regex]=men&price[lte]=15.99
Paginate
Default page=1 and limit=5
> GET /api/products?page=2
> GET /api/products?page=2&limit=7
Sort
Default sort='-createdAt'
> GET /api/products?sort=price
> GET /api/products?sort=createdAt
Full-text search
> GET /api/products?search=men