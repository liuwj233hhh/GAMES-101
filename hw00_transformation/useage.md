# 向量的使用
https://eigen.tuxfamily.org/dox/group__TutorialMatrixClass.html

类型定义：
```cpp
typedef Matrix<float, 3, 1> Vector3f;
typedef Matrix<int, 1, 2> RowVector2i;
typedef Matrix<double, Dynamic, Dynamic> MatrixXd;
typedef Matrix<int, Dynamic, 1> VectorXi;

// 初始化
Eigen::MatrixXd m(2,2);
MatrixXcf a = MatrixXcf::Random(2,2);
cout << "Here is the matrix a\n" << a << endl;
//  转置
cout << "Here is the matrix a^T\n" << a.transpose() << endl;
// 共轭
cout << "Here is the conjugate of a\n" << a.conjugate() << endl;
// 共轭转置
cout << "Here is the matrix a^*\n" << a.adjoint() << endl;
// 点乘和叉乘
std::cout << "Dot product: " << v.dot(w) << std::endl;
double dp = v.adjoint()*w; // automatic conversion of the inner product to a scalar
std::cout << "Dot product via a matrix product: " << dp << std::endl;
std::cout << "Cross product:\n" << v.cross(w) << std::endl;
```
